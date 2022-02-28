<template>
  <section id="home">
    <section class="showcase-area" id="showcase">
      <div class="showcase-container">
        <h1 class="main-title" id="home">Leigh-Anne Bowers</h1>
        <p>Aspired Web Developer</p>

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
.home {
  /* background-image: ("https://i.postimg.cc/7hrVCmVP/new-back.jpg");
  background: linear-gradient(blue, pink); */
  background-image: linear-gradient(
      to bottom,
      rgba(245, 246, 252, 0.356),
      #e9621e83
    ),
    url("https://i.postimg.cc/mr8vtcKP/developback.jpg");
  background-position: cover;
  background-size: cover;
  height: 100vh;
}
/* ............//// Showcase styling ////......... */

.showcase-area {
  height: 50vh;
  background: linear-gradient(
      rgba(240, 240, 240, 0.144),
      rgba(201, 139, 88, 0.377)
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
  margin-top: 1.5em;
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
.copy {
  margin-right: 5%;
}
</style>

<style>
.home {
  /* background-image: ("https://i.postimg.cc/7hrVCmVP/new-back.jpg");
  background: linear-gradient(blue, pink); */
  background-image: linear-gradient(
      to bottom,
      rgba(245, 246, 252, 0.356),
      #e9621e83
    ),
    url("https://i.postimg.cc/d3bng3ff/newbackground.jpg");
  background-position: cover;
  background-size: cover;
  height: 100vh;
}
.content {
  width: 70%;
  text-align: center;
}

.content .logo {
  width: 13%;
  position: absolute;
  top: 1rem;
  left: 2vw;
}

.content h1 {
  font-size: 4.5em;
  font-family: "Raleway", sans-serif;
  font-weight: 900;
}

.content h2 {
  position: relative;
  top: -30px;
  font-weight: 200;
}

.content .social_icons {
  position: fixed;
  right: 2vw;
  bottom: 2vh;
}

.content .social_icons:before {
  content: "";
  width: 1px;
  height: 100%;
  background-color: var(--white);
  position: absolute;
  top: -100%;
}

.content .social_icons a {
  margin: 10px 0px;
  color: var(--white);
  display: block;
  text-decoration: none;
  font-size: 1.5em;
  transition: 0.5s;
}

.content .social_icons a:hover {
  color: var(--primary);
}

.arrow {
  text-align: center;
  margin: 1% 0;
}
.arrow .fa {
  color: var(--white);
  font-weight: 200;
  text-decoration: none;
}
.bounce {
  -webkit-animation: bounce 2s infinite;
  animation: bounce 2s infinite;
}
@-webkit-keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-30px);
  }
  60% {
    transform: translateY(-15px);
  }
}
@keyframes bounce {
  0%,
  20%,
  50%,
  80%,
  100% {
    transform: translateY(0);
  }
  40% {
    transform: translateY(-30px);
  }
  60% {
    transform: translateY(-15px);
  }
}

.content .button {
  position: relative;
  top: -10px;
}

.searchBox {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, 50%);
  border-radius: 40px;
  padding: 5px 10px;
  display: flex;
}

.searchBox:hover > .searchInput {
  width: 240px;
  padding: 10px;
}

.searchBox:hover > .searchButton {
  background: white;
  color: #2f3640;
}

.searchBox:hover {
  background: #2f3640;
}

.searchBox:hover > .searchButton:hover {
  background-color: var(--primary);
  border: 1px solid var(--primary);
  color: var(--white);
}

.searchButton {
  color: white;
  float: right;
  width: auto;
  padding: 10px 20px;
  border-radius: 40px;
  background: transparent;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: 0.4s;
  border: 0;
  font-style: normal !important;
  font-weight: 600;
  text-align: center;
  border: 1px solid var(--white);
}

.searchInput {
  border: none;
  background: none;
  outline: none !important;
  float: left;
  padding: 0;
  color: white;
  font-size: 16px;
  transition: 0.4s;
  width: 0px;
}

@media screen and (max-width: 1020px) {
  .content h1 {
    font-size: 2em;
  }
  .content h2 {
    position: relative;
    top: -10px;
  }
}

@media screen and (max-width: 820px) {
  .content {
    width: 100%;
    padding: 1rem;
  }
  .content .logo {
    width: 20%;
  }
  .content h1 {
    font-size: 1.5em;
  }
  .content h2 {
    position: relative;
    top: -10px;
  }
  .content .social_icons {
    position: absolute;
    width: 100%;
    right: 0vw;
    bottom: 1vh;
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .content .social_icons a {
    margin: 0 15px;
  }

  .content .social_icons:before {
    content: "";
    width: 0px;
    height: 0%;
    top: 00%;
  }

  .searchBox:hover > .searchInput {
    max-width: 90%;
    width: 90%;
    padding: 5px 6px;
  }
  .searchBox:hover > .searchButton {
    font-size: 13px;
    white-space: nowrap;
  }
  .searchBox:hover {
    display: flex;
    width: 100%;
  }
}
</style>