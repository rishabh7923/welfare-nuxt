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
                <a class="navbar-brand mr-10" href="/">
                    <img src="~assets/images/logo.png" />
                </a>

                <div class="navbar-nav ms-auto">
                    <NuxtLink class="nav-item nav-link" to="/">Home</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/about/">About Us</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/feedback/">Feedback</NuxtLink>
                    <NuxtLink class="nav-item nav-link" to="/tour/">Tour</NuxtLink>
                </div>
                <div id="mobile-nav">
                    <font-awesome-icon class="m-2" v-b-toggle.sidebar-right icon="bars"
                        style="font-size: 30px;color:white;" />

                    <b-sidebar id="sidebar-right" title="Navigation" backdrop right shadow>
                        <div class="px-3 py-2">
                            <b-button href="/" class="mb-1" variant="light" style="width:100%;">Home</b-button>
                            <b-button href="/about" class="mb-1" variant="light" style="width:100%;">About Us</b-button>
                            <b-button href="/feedback" class="mb-1" variant="light" style="width:100%;">Feedback
                            </b-button>
                            <b-button href="/tour" class="mb-1" variant="light" style="width:100%;">Tour</b-button>
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
    width: 60px;
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
        background-color: #009ed6;
    }

    .b-sidebar-body button {
        color: var(--dark-gray);
    }

    .b-sidebar-header button {
        border: none;
        background-color: transparent;
        font-size: 30px;
        padding: 0px;
    }

    .b-sidebar-header button svg {
        color: var(--gray);
        font-weight: bold;
        font-size: 30px;
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