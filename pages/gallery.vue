<template>
    <main>
        <Header />
        <div class="container pt-3">
            <h4 class="heading">GALLERY OF MEMORIES</h4>
            <div class="divider"><span></span></div>
        </div>

        <div id="gallery" class="container bg-stylish rounded pb-3 pt-2">
            <div class="row row-cols-1 row-cols-md-5 g-4">
                <div class="col" v-for="(image, index) in imagesLoaded" :key="index">
                    <a target="_blank" :href="image.replace('m.jpg', '_d.webp?maxwidth=760&fidelity=grand')">
                        <img style="height:10rem;width: 100%;object-fit:cover;" class="rounded img-fluid"
                            :src="image" :alt="index">
                    </a>
                </div>
            </div>
        </div>
        <div class="container pagination justify-content-center pt-3 m-auto p-1">
            <b-button :disabled="length > images.length" @click="more">MORE</b-button>
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
            length: 20,
            images: require("../assets/gallery.json")
        }
    },
    methods: {
        more() {
            this.length += 20
        }
    },
    computed: {
        imagesLoaded() {
            return this.images.slice(0, this.length);
        }
    }
}
</script>