<template>
  <section id="home">
    <section class="showcase-area" id="showcase">
      <div class="showcase-container">
        <div class="container">
          <div class="row">
            <h1 class="main-title" id="home">Leigh-Anne Bowers</h1>
            <h3 class="animate-charcter">Aspired Web Developer</h3>
          </div>
        </div>
        <!-- <h1 class="main-title" id="home">Leigh-Anne Bowers</h1>
        <p>Aspired Web Developer</p> -->
        <!-- /////////////// -->
        <!-- <div class="container">
          <svg viewBox="0 0 1000 400">
            <text id="mytext" x="50%" y="50%" text-anchor="middle" fill="none">
              <p>Aspired Web Developer</p>
            </text>
            <use xlink:href="#mytext" class="copy copy1"></use>
            <use xlink:href="#mytext" class="copy copy2"></use>
            <use xlink:href="#mytext" class="copy copy3"></use>
            <use xlink:href="#mytext" class="copy copy4"></use>
            <use xlink:href="#mytext" class="copy copy5"></use>
          </svg>
        </div> -->
        <!-- ///////////////////// -->
        <div class="social_links">
          <a href="https://github.com/LeighBowers">
            <span class="fa-stack fa-lg fb combo">
              <i class="fa fa-circle fa-stack-2x circle"></i>
              <i class="fa fa-github fa-stack-1x fa-inverse icon"></i>
            </span>
          </a>

          <a href="https://codepen.io/leighbowers">
            <span class="fa-stack fa-lg gt combo">
              <i class="fa fa-circle fa-stack-2x circle"></i>
              <i class="fa fa-codepen fa-stack-1x fa-inverse icon"></i>
            </span>
          </a>
          <a href="https://www.linkedin.com/in/leigh-anne-sylvester-2752a421a/">
            <span class="fa-stack fa-lg tw combo">
              <i class="fa fa-circle fa-stack-2x circle"></i>
              <i class="fa fa-linkedin fa-stack-1x fa-inverse icon"></i>
            </span>
          </a>
          <!-- <a href="https://app.netlify.com/teams/leighbowers/overview">
        <span class="fa-stack fa-lg tw combo">
          <i class="fa fa-circle fa-stack-2x circle"></i>
       <a href="https://iconscout.com/icons/netlify" ></a> 

        </span>
      </a> -->
        </div>
      </div>
    </section>
  </section>
</template>

<script>
</script>


<style>
/* animation */
.animate-charcter {
  text-transform: uppercase;
  background-image: linear-gradient(
    -225deg,
    #3d0d3f 0%,
    #118032 29%,
    #114d7e 67%,
    #265088 100%
  );
  background-size: auto auto;
  background-clip: border-box;
  background-size: 200% auto;
  color: #fff;
  background-clip: text;
  text-fill-color: transparent;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  animation: textclip 2s linear infinite;
  display: inline-block;
  font-size: 31px;
}

@keyframes textclip {
  to {
    background-position: 200% center;
  }
}

.showcase-area {
  height: 100vh;
  background: linear-gradient(
      rgba(240, 240, 240, 0.144),
      rgba(88, 118, 201, 0.377)
    ),
    url("https://i.postimg.cc/yd1s7V0n/devel.jpg");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}

.showcase-container {
  display: flex;
  margin-right: 40%;
  padding-bottom: 10%;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
  font-size: 1.6rem;
}

.main-title {
  text-transform: uppercase;
  margin-top: 2.8em;
}
/* footer */
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&display=swap");

.social_links {
  padding: 1rem;

  margin-top: 2rem;

  flex-wrap: wrap;
  justify-content: center;
}
.social_links .combo {
  transform: scale(0.9);
  transition: 0.4s ease-in;
  margin: 0 0.5rem;
  height: 3em;
  width: 3em;
  line-height: 3em;
}
.combo .circle {
  color: #f9f9f9;
  transition: 0.4s ease-in;
  font-size: 3em;
}
.combo .icon {
  color: #444343;
  font-size: 2rem;
  transform: translateY(1px);
  transition: 0.2s ease-in;
}
.combo:hover {
  transform: scale(1.1);
}
.combo:hover,
.combo:hover .icon {
  color: white;
}

.fb:hover,
.fb:hover .circle {
  color: #10151a;
}

.tw:hover,
.tw:hover .circle {
  color: #191f24;
}
.gt:hover,
.gt:hover .circle {
  color: #1f1f1f;
}
/* .copy {
  margin-right: 5%;
} */
</style>

