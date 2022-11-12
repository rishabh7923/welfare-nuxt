<template>
    <main>
        <Header />
        <div class="container mt-3">
            <div>
                <h4 class="heading">CONTACT US</h4>
                <div class="divider"><span></span></div>
            </div>
        </div>

        <div class="container">
            <div class="row row-cols-1 row-cols-md-1 p-2 gap-5">
                <div class="col-md-4">
                    <ul class="list-unstyled">
                        <li class="bg-stylish rounded p-2">
                            <font-awesome-icon class="me-1" icon="location-dot" style="font-size: 19px" />
                            381, Shivli Road (Near Eldeco Jawaharpuram), Maqsoodabad, Kanpur-209217
                        </li>

                        <li class="bg-stylish rounded p-2 mt-2">
                            <font-awesome-icon class="me-1" icon="square-phone" style="font-size: 19px" />
                            +91-512-2070683
                        </li>

                        <li class="bg-stylish rounded p-2 mt-2">
                            <font-awesome-icon class="me-1" icon="square-phone" style="font-size: 19px" />
                            +91-9415892997
                        </li>

                        <li class="bg-stylish rounded p-2 mt-2">
                            <font-awesome-icon class="me-1" icon="envelope" style="font-size: 19px" />
                            info@welfareinternationalschool.org
                        </li>

                        <li class="bg-stylish rounded p-2 mt-2">
                            <font-awesome-icon class="me-1" icon="hashtag" style="font-size: 19px" />
                            <a
                                href="https://www.facebook.com/welfaremissioninternationalschool/">welfaremissioninternationalschool</a>
                        </li>
                    </ul>

                </div>

                <div class="col-md-7 p-0">
                    <b-skeleton-wrapper :loading="loading">
                        <template #loading>
                            <b-skeleton-img height="30rem"></b-skeleton-img>
                        </template>

                        <iframe class="rounded w-100" style="height: 30rem;"
                                src="https://maps.google.com/maps?q=381%2C%20New%20Shivli%20Rd%2C%20near%20ELDECO%2C%20Jawahar%20Puram%2C%20Masoodabad%2C%20Kanpur%2C%20Uttar%20Pradesh%2020921&t=m&z=10&output=embed&iwloc=near"></iframe>
                    </b-skeleton-wrapper>
                </div>
            </div>
        </div>
        <Footer />
    </main>
</template>

<script>
export default {
    data() { 
        return { loading: true } 
    },
    mounted() { setTimeout(() => this.loading = false, 1000) }
}
</script>