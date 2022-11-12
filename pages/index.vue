<template>
  <main>
    <Header />
    <!-- Slides -->
    <div id="slides" class="container animate slide">
      <b-skeleton-wrapper :loading="loading">
        <template #loading>
          <b-skeleton-img no-aspect height="340px"></b-skeleton-img>
        </template>

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
      </b-skeleton-wrapper>
    </div>

    <!-- About school section -->
    <div class="mt-3 rounded p-3 row m-auto container bg-stylish animate slide" id="about-school">
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

        <NuxtLink to="about" class="button ps-4 pe-4 float-end readmore rounded">Read More</NuxtLink>
      </div>
    </div>

    <div class="mt-3 rounded p-3 m-auto container bg-stylish" id="about-school">
      <p class="mt-2 fw">
        The Central Board of Secondary Education (CBSE) is a national level board of education in India for public and
        private schools, controlled and managed by the Government of India
        which is why <span class="fw-bold">Welfare Mission International School is officially affiliated to CBSE Board,
          New Delhi</span>
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
            <img src="https://i.imgur.com/0mYI9Yl.jpg" class="card-img" alt="Computer Lab"
              style="height: 100%; object-fit: cover;" />

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">COMPUTER LAB</p>
            </div>
          </div>
        </div>

        <div class="col-md-4">
          <div class="card h-100">
            <img src="https://i.imgur.com/8ScC3ix.jpg" class="card-img" alt="Lab class"
              style="height: 100%; object-fit: cover;">

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">LABORATORIES</p>
            </div>
          </div>
        </div>

        <div class="col-md-3 w-100">
          <div class="card h-100">
            <img src="https://i.imgur.com/yRePI1e.jpg" class="card-img" alt="Kids playing"
              style=" height: 15rem; object-fit: cover;" />

            <div class="card-img-overlay text-white text-end" style="opacity:0.8;">
              <p class="badge">PLAYGROUND</p>
            </div>
          </div>
        </div>
      </div>
    </div>


    <div id="events" class="container mt-3">
      <h4 class="heading">Events</h4>
      <div class="divider"><span></span></div>

      <div class="row row-cols-1 row-cols-md-4 g-4">

        <div class="col">
          <div class="card h-100">
            <img src="https://i.imgur.com/HepwNJE.jpg" class="card-img" alt="Kids Dressed on Janmashtami">

            <div class="card-img-overlay">
              <h5 class="card-title badge">Janmashtami</h5>
            </div>
          </div>
        </div>


        <div class="col">
          <div class="card h-100">
            <img src="https://i.imgur.com/2PqkKcw.jpg" class="card-img" alt="National Unity Day">

            <div class="card-img-overlay">
              <h5 class="card-title badge">National Unity Day</h5>
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
      <div class="row row">
        <div class="col-md-6">
          <h4 class="heading">GALLERY</h4>
          <div class="divider"><span></span></div>

          <div class="bg-stylish row pt-3 p-2 rounded">
            <div v-for="image in images" class="col-md-4">
              <img class="img-fluid mb-2 rounded w-100" style="object-fit:cover;height: 10rem;width: 20rem;"
                :src="image">
            </div>

            <div class="col-md-12 mt-2">
              <NuxtLink to="gallery"><button style="width: 10rem;height: 10rem;`"
                  class="img-fluid p-1 rounded w-100 more-button">MORE</button></NuxtLink>
            </div>
          </div>


        </div>

        <div class="col-md-6">
          <h4 class="heading">NOTICE</h4>
          <div class="divider"><span></span></div>

          <div class="">
            <ul class="list-unstyled">
              <li v-for="note in notices" class="bg-stylish p-2 rounded mt-2">
                <span><b>{{ note.title }}:</b> {{ note.description }}</span>
              </li>
            </ul>
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
  data() {
    return {
      loading: true,
      images: require("../assets/gallery.json").slice(0, 6),
      notices: [
        { title: "GURUNANAK JAINTI", description: "It is informed that school will remains closed on 08/11/22 , Tuesday on account of Guru Nanak jayanti." },
        { title: "DIWALI", description: "Wishing you all a very Happy Diwali, All of you are informed that from Monday to 27/10/2022, there will be a holiday in the school on the occasion of Diwali, Govardhan Puja and Bhai Dooj from 24/10/2022." },
        { title: "EXTRA CLASS", description: "Tomorrow extra class of physics for section A students will commence from 10:00-12:00  at Welfare mission public school on date 15/10/2022" },
        { title: "TIME CHANGE", description: "Buses will depart at 6:30 am Sharp from Welfare Mission Public School [Tomorrow, dated:1.10.2022 onwards]" },
        { title: "DURGA PUJA", description: "Please note that the school will remain closed on 02.10.2022 to 05.10.2022 on account of  Gandhi jayanti, Durga Puja,Mahanavami and Vijay Dashmi." },
        { title: "HEAVY RAINFAILL", description: "Please note that due to heavy rainfall the District Magistrate has issued an official order for the closure of all the schools of Kanpur city ." },
        { title: "WINTER", description: "The Winter Uniform will be applicable from 1 November 2022. Therefore every student are required to come in proper Winter Uniform otherwise a disciplinary action may be taken for non compliance." },
      ]
    }
  },
  head: {
    link: [
      { rel: "stylesheet", href: "/css/index.css" }
    ]
  },
  mounted() {
    setTimeout(() => this.loading = false, 200)
  }
}
</script>
