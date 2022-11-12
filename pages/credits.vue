<template>
    <main>
        <Header />
        <div class="container mt-3">
            <h1 class="heading">CREDITS</h1>
            <div class="divider"><span></span></div>

            <div class="row bg-stylish p-2 rounded pt-3 pb-3 credits shadow-sm">
                <div class="col-md-2 card">
                    <img class="rounded w-100" src="~assets/images/rishabh.jpg">

                    <div class="card-img-overlay">
                        <h5 class="card-title badge mb-2">DEVELOPER</h5>
                    </div>
                </div>

                <div class="col-md-10 ps-4">
                    <span class="heading mt-2">Rishabh Yadav</span>
                    <div class="divider mb-2"><span></span></div>

                    <p class="mb-2">Hello I'm a self-taught fullstack developer specialized in chat bot and website
                        development
                        with great
                        knowledge, and experience in discord.js, vue.js, nuxt, etc. I'm also great in JavaScript and Node.js. I'm
                        a student and still attending school, I am also creating video content for my audience on my
                        Youtube Channel so that i can learn more things while teaching others :)</p>
                </div>
            </div>

            <div class="row bg-stylish p-2 rounded pt-3 pb-3 mt-3 credits shadow-sm">
                <div class="col-md-10">
                    <h3 class="heading">Yash Jaiswal</h3>
                    <div class="divider mb-2"><span></span></div>

                    <p>My forte is 3D Animation and Modeling, I am proficient in Blender 3D and GIMP, and I can create
                        High End Visuals and Realistic Animated Videos.
                    </p>
                </div>

                <div class="col-md-2 card">
                    <img class="rounded img-fluid w-100" src="~assets/images/yash.jpg">

                    <div class="card-img-overlay text-end">
                        <h5 class="card-title badge mb-2">MODEL DESIGNER</h5>
                    </div>
                </div>
            </div>

            <div class="row bg-stylish p-2 rounded pt-3 pb-3 mt-3 credits shadow-sm">
                <div class="col-md-2 card">
                    <img class="rounded img-fluid w-100" src="~assets/images/anurag.jpg">
                    <div class="card-img-overlay">
                        <h5 class="card-title badge mb-2">EDITOR</h5>
                    </div>
                </div>

                <div class="col-md-9 ps-4">
                    <h3 class="heading mt-1">Anurag Saini</h3>
                    <div class="divider mb-2"><span></span></div>

                    <p>The photos on this website are edited by me; in addition to editing photos, I have a year's
                        experience programming Python; I also have several other skills such as arts and graphic design.
                    </p>
                </div>
            </div>

            <div class="row bg-stylish p-2 rounded pt-3 pb-3 mt-3 credits shadow-sm">
                <div class="col-md-10">
                    <h3 class="heading">Yogesh Singh</h3>
                    <div class="divider mb-2"><span></span></div>

                    <p>I excel at setting clear, measurable goals and leading cross-functional teams to deliver
                        meaningful outcomes. I am skilled in gathering information, interpreting data, identifying
                        opportunities, connecting teams, assigning resources, and delivering results.</p>
                </div>

                <div class="col-md-2 card">
                    <img class="rounded img-fluid w-100" src="~assets/images/yogesh.jpg">

                    <div class="card-img-overlay text-end">
                        <h5 class="card-title badge mb-2">PRODUCT MANAGER</h5>
                    </div>
                </div>
            </div>

            <div class="row bg-stylish p-2 rounded pt-3 pb-3 mt-3 credits shadow-sm">
                <div class="col-md-2 card">
                    <img class="rounded img-fluid w-100" src="~assets/images/utkarsh.jpg">

                    <div class="card-img-overlay">
                        <h5 class="card-title badge mb-2">ASSET MANAGER</h5>
                    </div>
                </div>

                <div class="col-md-9 ps-4">
                    <h3 class="heading mt-1">Utkarsh Jaiswal</h3>
                    <div class="divider mb-2"><span></span></div>

                    <p>Hello, I'm Utkarsh Jaiswal. The skills I have are Graphic Designing, Video Editing,
                        Cinematography, and Film Making. I have almost 1.5 years of experience in each area. </p>
                </div>
            </div>
        </div>
        <Footer />
    </main>
</template>

<style>
.credits img {
    width: 10rem;
    object-fit: cover;
    height: 10rem;
}

.credits .card div.card-img-overlay {
    position: absolute;
    top: -5px;
    right: 0;
    bottom: 0;
    left: 0;
    padding: 0px;
    font-size: 10px
}

.credits .card .badge {
    font-size: 10px;
}

.credits .card {
    border: none;
    background-color: transparent;
}
</style>