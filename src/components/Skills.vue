<template>
  <section id="skills">
    <div class="skill-title"><h1>Skills</h1></div>
    <div class="skills">
      <div class="skills-container">
        <div class="row">
          <div class="col-lg">
            <div class="box">
              <i class="fas fa-mouse fa-3x mb-4"></i>
              <h4>Web Design</h4>
              <p>
                Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
                Sed id mauris vel neque
              </p>
              <a class="readmore" href="#"><span>Read More</span></a>
            </div>
          </div>

          <div class="col-lg">
            <div class="box">
              <i class="fas fa-laptop-code fa-3x mb-4"></i>
              <h4>Coding</h4>
              <p>
                Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
                Sed id mauris vel neque
              </p>
              <a class="readmore" href="#"><span>Read More</span></a>
            </div>
          </div>
          <div class="col-lg">
            <div class="box">
              <i class="fas fa-mobile-alt fa-3x mb-4"></i>
              <h4>App Developing</h4>
              <p>
                Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
                Sed id mauris vel neque
              </p>
              <a class="readmore" href="#"><span>Read More</span></a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
/* body {
  background: linear-gradient(to bottom, rgba(245, 246, 252, 0.356), #e9621e83),
    url("");
  background-position: cover;
  background-size: cover;
  height: 100vh;
} */
.skills {
  margin-top: 50px;
  width: 100%;
}
.skill-title {
  position: relative;
  padding-bottom: 2px;
}
.skill-title {
  position: relative;
  color: #e9621eec;
  font-size: 18px;
  font-weight: 700;
  padding-right: 50px;
  margin-bottom: 15px;
  display: inline-block;
  text-transform: capitalize;
}
.skill-title :before {
  position: absolute;
  content: "";
  right: 0px;
  bottom: 7px;
  width: 40px;
  height: 1px;
  background-color: #d66e28;
}
.skills .box {
  background-color: #0e409c48;
  overflow: hidden;
  transition: 0.3s ease;
  left: 25px;
  position: relative;
  padding-top: 5px;
}
.skills .box i {
  color: #e9621eec;
  transition: inherit;
  transition-delay: 0s;
}
.skills h4 {
  color: rgb(2, 27, 61);
  transition: inherit;
  transition-delay: 0.05s;
}
.skills p {
  color: #06023f;
  transition: inherit;
  transition-delay: 0.1s;
}
.readmore {
  color: rgb(13, 2, 61);
  overflow: hidden;
  display: inline-block;
  font-size: 0.75rem;
  text-transform: uppercase;
  font-weight: 700;
  color: rgb(1, 0, 80);
  position: relative;
  padding-right: 2rem;
}
.readmore:before {
  animation: ts-link-arrow-effect-animation-out;
  animation-fill-mode: forwards;
  animation-duration: 0.4s;
  animation-timing-function: cubic-bezier(0.6, 0.01, 0, 1);
  background-color: #f26c4f;
  bottom: 0;
  height: 0.125rem;
  margin: auto;
  left: 0;
  content: "";
  position: absolute;
  top: 0;
  width: 100%;
  transform: scaleX(0.2);
  transform-origin: left center;
  z-index: 0;
}
.readmore span {
  position: relative;
  transform: translateX(-200%);
  display: inline-block;
  transition: 0.6s cubic-bezier(0.6, 0.01, 0, 1);
}
.box:hover .readmore span {
  transform: translateX(0%);
}
.box:hover .readmore:before {
  animation: ts-link-arrow-effect-animation-in;
  animation-fill-mode: forwards;
  animation-duration: 0.4s;
  animation-timing-function: cubic-bezier(0.6, 0.01, 0, 1);
}
.box:hover i,
.box:hover h4,
.box:hover p {
  transform: translateY(-0.625rem);
}
@keyframes ts-link-arrow-effect-animation-out {
  0% {
    transform-origin: right center;
    transform: scaleX(0.2);
  }

  70% {
    transform-origin: right center;
  }

  71% {
    transform-origin: left center;
    transform: scaleX(1);
  }

  100% {
    transform-origin: left center;
    transform: scaleX(0.2);
  }
}
@keyframes ts-link-arrow-effect-animation-in {
  0% {
    transform-origin: left center;
    transform: scaleX(0.2);
  }

  70% {
    transform-origin: left center;
    transform: scaleX(1);
  }

  71% {
    transform-origin: right center;
  }

  100% {
    transform-origin: right center;
    transform: scaleX(0.2);
  }
}
</style>