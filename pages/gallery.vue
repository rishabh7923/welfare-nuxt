<template>
    <main>
        <Header />
        <div class="container pt-3">
            <h4 class="heading">GALLERY OF MEMORIES</h4>
            <div class="divider"><span></span></div>
        </div>

        <div id="gallery" class="container bg-stylish rounded pb-3 pt-2">
            <div class="row row-cols-1 row-cols-md-5 g-4">
                <div class="col" v-for="index in 20">
                    <a target="_blank"
                        :href="images[index].replace('m.jpg', '_d.webp?maxwidth=760&fidelity=grand')"><img
                            v-if="images[index + (page * 20)]" style="height:10rem;width: 100%;object-fit:cover;"
                            class="rounded img-fluid" :src="images[index + (page * 20)]" :alt="index">
                    </a>
                </div>
            </div>
        </div>
        <div class="container pagination justify-content-center pt-3 m-auto p-1">
            <b-button :disabled="images[(page - 1) * 20] ? false : true" @click="previous">Previous Page</b-button>
            <b-button :disabled="images[(page + 1) * 20] ? false : true" @click="next">Next Page</b-button>
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
        console.log(this.images)
    },
    methods: {
        previous() {
            this.page = this.page - 1
            window.scrollTo(0, 0)
        },

        next() {
            this.page = this.page + 1
            window.scrollTo(0, 0)
        }
    }
}
</script>