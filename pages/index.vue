<template>
  <main>
    <Header />
    <!-- Slides -->
    <div id="slides" class="carousel container" data-bs-ride="carousel">
      <!-- The slideshow/carousel -->
      <div class="carousel-inner carousel-fade mt-2 rounded m-auto">
        <div class="carousel-item active">
          <img src="http://welfareinternationalschool.org/images/gallery/7.jpg" alt="first"
            class="d-block w-100 img-container">
          <div class="carousel-caption d-none d-md-block">
            <h5>EDUCATION MATTERS</h5>
          </div>
        </div>

        <div class="carousel-item">
          <img src="http://welfareinternationalschool.org/images/gallery/4.jpg" alt="second" class="d-block w-100">

          <div class="carousel-caption d-none d-md-block">
            <h5>OUR MISSION</h5>
          </div>
        </div>

        <div class="carousel-item">
          <img src="http://welfareinternationalschool.org/images/gallery/3.jpg" alt="third" class="d-block w-100">
          <div class="carousel-caption d-none d-md-block">
            <h5>LEARN AND GROW</h5>
          </div>
        </div>
      </div>
    </div>

    <!-- About school section -->
    <div class="mt-3 rounded p-3 row m-auto container bg-stylish" id="about-school">
      <div class="col-md-4">
        <img src="https://welfareinternationalschool.org/images/about.jpg" alt="My Image" class="img-fluid rounded">
      </div>
      <div class="col-md-7">
        <p class="mt-2">
          <span class="underline">Welfare Mission Educational Society</span> was founed by CA Raj Shiromani Singh
          and Mrs. Veena Singh inspired
          by the teachings of eminent personalities like Mahatma Buddha, Ravindra Nath Tagore and Dr. Sarvepalli
          Radha Krishnan.
        </p>
        <p>
          The founders established their first school in 2004 with a mission to provide quality education without
          any discrimination and compromise, with all the best possible facilities of international standards
          through English as a medium of instruction, to the aspirant children belonging to a class of society who
          are not able to afford costly and a decent education, because here at <span class="underline">Welfare
            Mission</span> we believe that:
        </p>
        <p class="fst-italic fw-bold">
          <i class="fa fa-quote-left fa-pull-left"></i>Education is matter of faith and trust not of money and prestige.
        </p>

        <a href="#" class="button ps-4 pe-4 float-end readmore rounded">Read More</a>
      </div>
    </div>

    <!-- Facilities -->
    <div id="facility" class="container mt-3">
      <h4>Facilities</h4>
      <div class="row row-cols-1 row-cols-md-3 g-3">
        <div class="col-md-5">
          <div class="card h-100">
            <img src="~assets/images/2.jpg" class="card-img" alt=".." style=" height: 100%; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">SPORTS</p>
            </div>
          </div>
        </div>

        <div class="col-md-3">
          <div class="card h-100">
            <img src="https://christelhouse.org/images/stories/1501087250_INDIA-LAB-RETOUCHED.jpg" class="card-img"
              alt=".." style="height: 100%; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">COMPUTER LAB</p>
            </div>
          </div>
        </div>

        <div class="col-md-4">
          <div class="card h-100">
            <img src="http://regionalbikeplan.org/wp-content/uploads/2019/02/Music-Room-img5-1.jpg" class="card-img"
              alt=".." style=" height: 100%; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">MUSIC</p>
            </div>
          </div>
        </div>

        <div class="col-md-3 w-100">
          <div class="card h-100">
            <img
              src="https://images.edexlive.com/uploads/user/imagelibrary/2019/10/14/original/indian-asian-boy-swimming-spool-260nw-152203244.jpg"
              class="card-img" alt=".." style=" height: 15rem; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">SWIMMING</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container mt-3">
      <h4>Events</h4>
      <div class="row row-cols-1 row-cols-md-3 g-4">

        <div class="col">
          <div class="card h-100">
            <img src="~assets/images/3.jpeg" class="card-img" alt="...">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Earth Day</h5>
            </div>
          </div>
        </div>


        <div class="col">
          <div class="card h-100">
            <img src="~assets/images/4.jpeg" class="card-img" alt="...">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Dusheraa</h5>
            </div>
          </div>
        </div>


        <div class="col">
          <div class="card h-100">
            <img src="~assets/images/5.jpeg" class="card-img" alt="...">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Independence Day</h5>
            </div>
          </div>
        </div>

      </div>
    </div>

    <div class="container mt-3">
      <h3>Contact Us</h3>
      <div id="contact-form" class="rounded mt-2 p-3 bg-stylish">
        <div class="row g-2">
          <div class="col">
            <img class="float-start rounded img-fluid" src="~assets/images/1.jpg" alt="Enterance Image">
          </div>

          <div class="col-md-8">
            <div class="row g-2">
              <div class="col">
                <div class="form-floating">
                  <input class="form-control" placeholder="Your good last name" id="floatingInput">
                  <label for="floatingInput">First Name</label>
                </div>
              </div>

              <div class="col">
                <div class="form-floating">
                  <input class="form-control" placeholder="Your good last name" id="floatingInput">
                  <label for="floatingInput">Last Name</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="col">
                <div class="form-floating">
                  <input type="email" class="form-control" placeholder="email address" id="floatingInput">
                  <label for="floatingInput">Email Address</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="col">
                <div class="form-floating">
                  <input type="email" class="form-control" placeholder="email address" id="floatingInput">
                  <label for="floatingInput">Phone Number</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="form-floating">
                <div class="form-floating">
                  <input type="email" class="form-control" placeholder="email address" id="floatingInput">
                  <label for="floatingInput">Reason</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="form-floating">
                <textarea class="form-control" placeholder="email address to contact you" id="floatingInput"
                  style="height: 150px"></textarea>
                <label for="floatingInput">How can we help you?</label>
              </div>
            </div>

            <button type="submit" class="btn btn-secondary mt-2 float-end w-100">Send Message</button>
          </div>

        </div>
      </div>
    </div>
    
    <Footer />
  </main>
</template>

<script>
export default {
  name: 'IndexPage',
  head: {
    link: [
      { rel: "stylesheet", href: "/css/index.css" }
    ]
  }
}
</script>
