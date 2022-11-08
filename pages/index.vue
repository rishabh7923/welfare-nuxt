<template>
  <main>
    <Header />
    <!-- Slides -->
    <div id="slides" class="container">
      <b-carousel class="carousel-fade" id="carousel" :interval="4000" img-width="1024" img-height="480" controls>

        <b-carousel-slide img-alt="Education Matters" img-src="https://i.imgur.com/yJwGLPf.jpg">
          <h3>EDUCATION MATTERS</h3>
        </b-carousel-slide>

        <b-carousel-slide img-alt="Our Mission" img-src="https://i.imgur.com/3rNlkKc.jpg">
          <h3>OUR MISSION</h3>
        </b-carousel-slide>

        <b-carousel-slide img-alt="Learn And Grow" img-src="https://i.imgur.com/Rlq7L41.jpg">
          <h3>LEARN AND GROW</h3>
        </b-carousel-slide>
      </b-carousel>
    </div>

    <!-- About school section -->
    <div class="mt-3 rounded p-3 row m-auto container bg-stylish" id="about-school">
      <div class="col-md-4">
        <img src="https://i.imgur.com/woRlMqd.jpg" alt="School Main Door" class="img-fluid rounded">
      </div>
      <div class="col-md-7">
        <p class="mt-2">
          <span class="underline">Welfare Mission Educational Soociety</span> was founed by CA Raj Shiromani Singh
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

        <a href="about" class="button ps-4 pe-4 float-end readmore rounded">Read More</a>
      </div>
    </div>

    <div class="mt-3 rounded p-3 m-auto container bg-stylish" id="about-school">
        <p class="mt-2 fw">
          The Central Board of Secondary Education (CBSE) is a national level board of education in India for public and private schools, controlled and managed by the Government of India
          which is why <span class="fw-bold">Welfare Mission International School is officially affiliated to CBSE Board, New Delhi</span>
          and affiliation number is 2131971
        </p>
    </div>

    <!-- Facilities -->
    <div id="facility" class="container mt-3">
      <h4 class="heading">Facilities</h4>
      <div class="divider"><span></span></div>

      <div class="row row-cols-1 row-cols-md-3 g-3">
        <div class="col-md-5">
          <div class="card h-100">
            <img src="https://i.imgur.com/8Nxv58N.jpg" class="card-img" alt="Sports"
              style="height: 100%; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">SPORTS</p>
            </div>
          </div>
        </div>

        <div class="col-md-3">
          <div class="card h-100">
            <img src="https://i.imgur.com/0mYI9Yl.jpg" class="card-img" alt="Computer Lab" style="height: 100%; object-fit: cover;" />

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">COMPUTER LAB</p>
            </div>
          </div>
        </div>

        <div class="col-md-4">
          <div class="card h-100">
            <img src="https://i.imgur.com/8ScC3ix.jpg" class="card-img" alt="Lab class" style="height: 100%; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">LABORATORIES</p>
            </div>
          </div>
        </div>

        <div class="col-md-3 w-100">
          <div class="card h-100">
            <img src="https://i.imgur.com/UEOeBb8.jpg" class="card-img" alt="Kids playing" style=" height: 15rem; object-fit: cover;" />

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">PLAYGROUND</p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Affiliated to CBSE -->






    <div id="events" class="container mt-3">
      <h4 class="heading">Events</h4>
      <div class="divider"><span></span></div>

      <div class="row row-cols-1 row-cols-md-4 g-4">

        <div class="col">
          <div class="card h-100">
            <img src="https://i.imgur.com/HepwNJE.jpg" class="card-img" alt="Kids Dressed on Janmashtami" >

            <div class="card-img-overlay">
              <h5 class="card-title badge">Janmashtami</h5>
            </div>
          </div>
        </div>


        <div class="col">
          <div class="card h-100">
            <img src="https://i.imgur.com/2PqkKcw.jpg" class="card-img" alt="National Unity Dat">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Natiional Unity Day</h5>
            </div>
          </div>
        </div>


        <div class="col">
          <div class="card h-100">
            <img src="https://i.imgur.com/tv7DWcv.jpg" class="card-img" alt="Independence Day">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Independence Day</h5>
            </div>
          </div>
        </div>

        <div class="col">
          <div class="card h-100">
            <img src="https://i.imgur.com/MbtpXW6.jpg" class="card-img" alt="Dussehra">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Dussehra</h5>
            </div>
          </div>
        </div>

      </div>
    </div>

    <div class="container mt-3">
      <h3 class="heading">Contact Us</h3>
      <div class="divider"><span></span></div>
      <div id="contact-form" class="rounded mt-2 p-3 bg-stylish">
        <div class="row g-2">
          <div class="col">
            <img class="float-start rounded img-fluid" src="https://i.imgur.com/u33G1BE.jpg" alt="Enterance Image" />
          </div>

          <div class="col-md-8">
            <div class="row g-2">
              <div class="col">
                <div class="form-floating">
                  <input class="form-control" placeholder="Your good last name" id="firstName">
                  <label for="firstName">First Name</label>
                </div>
              </div>

              <div class="col">
                <div class="form-floating">
                  <input class="form-control" placeholder="Your good last name" id="lastName">
                  <label for="lastName">Last Name</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="col">
                <div class="form-floating">
                  <input type="email" class="form-control" placeholder="email address" id="emailAddress">
                  <label for="emailAddress">Email Address</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="col">
                <div class="form-floating">
                  <input type="number" class="form-control" placeholder="Number" id="phoneNumber">
                  <label for="phoneNumber">Phone Number</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="form-floating">
                <div class="form-floating">
                  <input type="text" class="form-control" placeholder="Reason for Request" id="reason">
                  <label for="reason">Reason</label>
                </div>
              </div>
            </div>

            <div class="row g-2 mt-1">
              <div class="form-floating">
                <textarea class="form-control" placeholder="email address to contact you" id=""
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
