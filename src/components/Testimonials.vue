<template>
  <section id="testimonials">
    <div class="test-title"><h1>Testimonials</h1></div>
    <div class="container p-5">
      <div class="row row-cols-1 row-cols-xs-2 row-cols-sm-2 row-cols-lg-4 g-3">
        <div
          v-for="testimonial in testimonials"
          :key="testimonial.id"
          class="col"
        >
          <div class="test-card h-100 shadow-sm">
            <div class="text-center">
              <div class="img-hover-zoom img-hover-zoom--colorize">
                <img
                  class="shadow"
                  :src="testimonial.img"
                  alt="Another Image zoom-on-hover effect"
                />
              </div>
            </div>

            <div class="card-body">
              <div class="clearfix mb-3"></div>

              <div class="my-2 text-center">
                <h1>{{ testimonial.name }}</h1>
              </div>
              <div class="mb-3">
                <h2 class="text-uppercase text-center role">
                  {{ testimonial.desc }}
                </h2>
              </div>
            </div>
          </div>
        </div>
        <!-- <div class="col">
          <div class="test-card h-100 shadow-sm">
            <div class="text-center">
              <div class="img-hover-zoom img-hover-zoom--colorize">
                <img
                  class="shadow"
                  src="https://i.postimg.cc/ht2QBpf7/Cameron1.jpg"
                  alt="Another Image zoom-on-hover effect"
                />
              </div>
            </div>

            <div class="card-body">
              <div class="clearfix mb-3"></div>

              <div class="my-2 text-center">
                <h1>Cameron</h1>
              </div>
              <div class="mb-3">
                <h2 class="text-uppercase text-center role">
                  Leigh-Anne is a very kind and hardworking individual. she is
                  passionate about coding and very committed to her work. she
                  works well with others and is a good leader.
                </h2>
              </div>
            </div>
          </div>
        </div> -->
        <!-- <div class="col">
          <div class="test-card h-100 shadow-sm">
            <div class="text-center">
              <div class="img-hover-zoom img-hover-zoom--colorize">
                <img
                  class="shadow"
                  src="https://i.postimg.cc/y6MJ1Mf9/Craig3.jpg"
                  alt="Another Image zoom-on-hover effect"
                />
              </div>
            </div>

            <div class="card-body">
              <div class="clearfix mb-3"></div>

              <div class="my-2 text-center">
                <h1>Craig</h1>
              </div>
              <div class="mb-3">
                <h2 class="text-uppercase text-center role">
                  She is very sweet and a team player. She never shys away from
                  asking for help and helps out where she can too. Shes an
                  extremely hard worker and knows how to present a good website.
                </h2>
              </div>
            </div>
          </div>
        </div> -->
        <!-- <div class="col">
          <div class="test-card h-100 shadow-sm">
            <div class="text-center">
              <div class="img-hover-zoom img-hover-zoom--colorize">
                <img
                  class="shadow"
                  src="https://i.postimg.cc/LXjR4bQ4/Amaarah3.jpg"
                  alt="Another Image zoom-on-hover effect"
                />
              </div>
            </div>

            <div class="card-body">
              <div class="clearfix mb-3"></div>

              <div class="my-2 text-center">
                <h1>Amaarah</h1>
              </div>
              <div class="mb-3">
                <h2 class="text-uppercase text-center role">
                  Leigh-Anne is a great person to work with. She is very helpful
                  and considerate of others and she has a very good work ethic.
                  She would be a great addition to any team she is a part of. I
                  enjoy working with her.
                </h2>
              </div>
            </div>
          </div>
        </div> -->
        <!-- <div class="col">
          <div class="test-card h-100 shadow-sm">
            <div class="text-center">
              <div class="img-hover-zoom img-hover-zoom--colorize">
                <img
                  class="shadow"
                  src="https://i.postimg.cc/GhhwgzPT/Diego2.jpg"
                  alt="Another Image zoom-on-hover effect"
                />
              </div>
            </div>

            <div class="card-body">
              <div class="clearfix mb-3"></div>

              <div class="my-2 text-center">
                <h1>Diego</h1>
              </div>
              <div class="mb-3">
                <h2 class="text-uppercase text-center role">
                  Leigh-anne is very self motivated individual that pays close
                  attention to detail and always makes sure to get the job done
                  .
                </h2>
              </div>
            </div>
          </div>
        </div> -->
        <!-- <div class="col">
          <div class="test-card h-100 shadow-sm">
            <div class="text-center">
              <div class="img-hover-zoom img-hover-zoom--colorize">
                <img
                  class="shadow"
                  src="https://i.postimg.cc/0jZfp9Xt/Tursha4.jpg"
                  alt="Another Image zoom-on-hover effect"
                />
              </div>
            </div>

            <div class="card-body">
              <div class="clearfix mb-3"></div>

              <div class="my-2 text-center">
                <h1>Tursha</h1>
              </div>
              <div class="mb-3">
                <h2 class="text-uppercase text-center role">
                  This young women is extremely hard working.She never backs
                  down from a challege and always gives it her best.Overall a
                  lovely person to work with!
                </h2>
              </div>
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </section>
</template>


<script>
export default {
  data() {
    return {
      testimonials: [],
    };
  },
  mounted() {
    fetch("https://leigh-anne-api.herokuapp.com/testimonials")
      .then((res) => res.json())
      .then((data) => (this.testimonials = data))
      .catch((err) => console.log(err.message));
  },
};
</script>

<style>
#testimonials {
  margin-top: -100px;
}
.test-title {
  position: relative;
  padding-bottom: 2px;
}
.test-title {
  position: relative;
  color: #e9621eec;
  font-size: 18px;
  font-weight: 700;
  padding-right: 50px;
  margin-bottom: 15px;
  display: inline-block;
  text-transform: capitalize;
}
.test-title :before {
  position: absolute;
  content: "";
  right: 0px;
  bottom: 7px;
  width: 40px;
  height: 1px;
  background-color: #d66e28;
}

.container-fluid {
  max-width: 1400px;
}

.test-card {
  background: #9e9090bd;
  box-shadow: 0 6px 10px rgba(0, 0, 0, 0.08), 0 0 6px rgba(0, 0, 0, 0.05);
  border: 1;
  border-radius: 1rem;
}

.img-hover-zoom--colorize img {
  width: 150px;
  height: auto;
  margin-top: 20px;
  padding: 1px;
  transition: transform 0.5s;
  filter: grayscale(100%);
  align-items: center;
}

.img-hover-zoom--colorize:hover img {
  filter: grayscale(0);
  transform: scale(1.05);
}

.test-card h5 {
  overflow: hidden;
  height: 80px;
  font-weight: 300;
  font-size: 1rem;
}

.test-card h5 a {
  color: black;
  text-decoration: none;
}

.role {
  color: #7a7a7a;
}

.box {
  display: flex;
  align-items: center;
  justify-content: center;
}

.fab {
  font-size: 1.5rem;
  color: darkgray;
  transition: transform 0.5s;
}

.fab:hover {
  color: black;
  transform: scale(1.1);
}

.test-card h2 {
  font-size: 1rem;
}

/* MEDIA */

@media only screen and (min-width: 1200px) {
  .img-hover-zoom--colorize img {
    width: 200px;
  }
}

@media only screen and (min-width: 1200px) {
  .h1,
  h1 {
    font-size: 2rem;
  }
}
</style>
