<template>

    <div id="header" class="container" style="padding: 0px 0px">
        <div id="contact-strip">
            <NuxtLink to="/admission" class="tnav-item">
                <font-awesome-icon icon="school" style="font-size: 19px" />
                <span class="fw-bold pe-2">ADMISSION /</span>
            </NuxtLink>

            <NuxtLink to="/gallery" class="tnav-item">
                <font-awesome-icon icon="image" style="font-size: 19px" />
                <span class="fw-bold pe-2">GALLERY /</span>
            </NuxtLink>

            <a href="http://welfareinternationalschool.org/downloads/prospects.pdf" class="tnav-item">
                <font-awesome-icon icon="circle-down" style="font-size: 19px" />
                <span class="fw-bold pe-2">PROSPECTUS /</span>
            </a>

            <font-awesome-icon icon="square-phone" style="font-size: 19px" />
            <span class="fw-bold pe-2">+91-28282-1829782</span>

        </div>

        <nav class="navbar navbar-expand m-auto">
            <div class="container">
                <NuxtLink class="navbar-brand mr-10" to="/">
                    <img src="~assets/images/logo.png" />
                </NuxtLink>

                <div class="navbar-nav ms-auto">
                    <NuxtLink class="nav-item nav-link" to="/">HOME</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/mela/">MELA</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/about/">ABOUT</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/feedback/">FEEDBACK</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/contact/">CONTACT</NuxtLink>
                </div>
                <div id="mobile-nav">
                    <font-awesome-icon class="m-2" v-b-toggle.sidebar-right icon="bars"
                        style="font-size: 30px;color:white;" />

                    <b-sidebar id="sidebar-right" title="NAVIGATION" backdrop right shadow>
                        <div class="px-3 py-2">
                            <NuxtLink to="/" class="btn btn-light w-100 fw-bold">Home</NuxtLink>
                            <NuxtLink to="/about" class="btn btn-light w-100 fw-bold mt-1">About</NuxtLink>
                            <NuxtLink to="/feedback" class="btn btn-light w-100 fw-bold mt-1">Feedback</NuxtLink>
                            <NuxtLink to="/mela" class="btn btn-light w-100 fw-bold mt-1">Mela</NuxtLink>
                            <NuxtLink to="/contact" class="btn btn-light w-100 fw-bold mt-1">Contact</NuxtLink>
                            <NuxtLink to="/admission" class="btn btn-light w-100 fw-bold mt-1">Admission</NuxtLink>
                            <NuxtLink to="/gallery" class="btn btn-light w-100 fw-bold mt-1">Gallery</NuxtLink>
                        </div>
                    </b-sidebar>
                </div>
            </div>
        </nav>


    </div>
</template>

<style>
#header {
    padding: 10px;
    border-radius: 0px 0px 10px 10px;
    background-color: var(--primary)
}

#contact-strip {
    text-align: right;
    background-color: #027ca7;
    border-radius: 0px 0px 0px 20px;
    padding: 3px;
    width: 70%;
    margin-left: auto;
    color: var(--gray);
    font-size: 15px;
    font-family: monospace;
}

#mobile-nav {
    display: none;
}

.navbar-brand img {
    width: 125px;
    position: absolute;
    bottom: 10px;
}

.nav-item {
    color: var(--gray);
    font-family: monospace;
    padding: 0px;
}

.nav-item.nav-link.active {
    color: white;
    font-weight: bold;
    border-bottom: 3px solid var(--primary);
    border-image: linear-gradient(0.25turn, #73dbff, #74dbff, #2ab4e6);
    border-image-slice: 1;
}

.nav-link:focus,
.nav-link:hover {
    color: white;
}

div.navbar-nav .active {
    color: white;
}

.tnav-item {
    text-decoration: none;
    color: var(--gray);
}

.tnav-item:focus,
.tnav-item:hover {
    color: var(--gray);
}

@media (max-width: 991.98px) {
    #mobile-nav {
        display: block;
    }

    #contact-strip {
        display: none;
    }

    .navbar-nav {
        display: none;
    }

    .navbar-brand img {
        position: unset;
    }

    .b-sidebar-header,
    .b-sidebar-body {
        color: white;
        background-color: var(--primary);
        opacity: 0.6;
        background-image: radial-gradient(#d7d0d0 0.8px, #009ad0 0.8px);
        background-size: 16px 16px;
    }

    .b-sidebar-body a, .b-sidebar-body a:hover, .b-sidebar-body a:focus {
        color: #147a9d;
        background-color: #5bd2fc;
    }

    .b-sidebar-header a {
        border: none;
        background-color: transparent;
        font-size: 30px;
        padding: 0px;
    }

    .b-sidebar-header button {
        border: none;
        outline: none;
        background-color: transparent;
        font-weight: 20px;
    }

    .b-sidebar-header svg {
        font-weight: bold;
        font-size: 30px;
        background-color: #5bd2fc;
        border: none;
        color: white;
        border-radius: 5px;
    }
}

@media (max-width: 575.98px) {
    #header {
        border-radius: 0px;
    }
}
</style>

<script>
export default {
    mounted() {
        const element = document.querySelector(`.nav-item[href='${document.location.pathname}']`)
        element?.classList.add("active")
    }
}

</script>