<template>
    <main>
        <Header />
        <div id="gallery" class="container mt-5 bg-stylish rounded pb-3">
            <div class="row row-cols-1 row-cols-md-5 g-4">
                <div class="col" v-for="index in 20">
                    <a target="_blank" :href="images[index].replace('m.', '.')"><img v-if="images[index + (page * 20)]" style="height:10rem;width: 100%;object-fit:cover;"
                            class="rounded img-fluid" :src="images[index + (page * 20)]" :alt="index">
                    </a>
                </div>
            </div>
        </div>
        <div class="container pagination justify-content-center pt-3 m-auto p-1">
            <button :disabled="images[(page - 1) * 20] ? false : true" @click="page = page - 1">Previous Page</button>
            <button :disabled="images[(page + 1) * 20] ? false : true" @click="page = page + 1">Next Page</button>
        </div>

        <Footer />
    </main>
</template>

<style>
.pagination button {
    outline: none;
    border: none;
    background-color: var(--primary);
    color: var(--gray);
    padding: 10px;
    font-weight: bold;
    border-radius: 2px;
    width: 100%;
    margin: 2px;
}

.pagination button:disabled {
    filter: brightness(90%)
}
</style>

<script>
export default {
    data() {
        return {
            images: require("../assets/gallery.json"),
            page: null
        }
    },
    mounted() {
        this.page = this.$route.query.page ? this.$route.query.page - 1 : 0
        console.log((this.page * 10) + 0)
    }
}
</script>