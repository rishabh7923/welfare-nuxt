<template>
    <div id="header" class="container" style="padding: 0px 0px">
        <div id="contact-strip">
            <font-awesome-icon icon="school" style="font-size: 19px"/>
            <span class="fw-bold pe-2">ADMISSION /</span>

            <font-awesome-icon icon="image" style="font-size: 19px"/>
            <span class="fw-bold pe-2">GALLERY /</span>

            <font-awesome-icon icon="circle-down" style="font-size: 19px"/>
            <span class="fw-bold pe-2">PROSPECTUS /</span>

            <font-awesome-icon icon="square-phone" style="font-size: 19px"/>
            <span class="fw-bold pe-2">+91-28282-1829782</span>

        </div>

        <nav class="navbar navbar-expand m-auto">
            <div class="container">
                <a class="navbar-brand mr-10" href="#">
                    <img src="~/assets/images/logo.png">
                </a>

                <div class="navbar-nav ms-auto">
                    <a class="nav-item nav-link" href="/">Home</a>
                    <a class="nav-item nav-link" href="/about">About Us</a>
                    <a class="nav-item nav-link" href="/feedback">Feedback</a>
                    <a class="nav-item nav-link" href="/tour">Tour</a>
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

@media (max-width: 991.98px) {
    #contact-strip {
        display: none;
    }

    .navbar-nav {
        display: none;
    }

    .navbar-brand img {
        position: unset;
    }
}

@media (max-width: 575.98px) {
    #header {
        border-radius: 0px;
    }
}
</style>