<template>
  <div class="skills">
    <div class="container">
      <div class="row">
        <div class="col-md-6 col-lg-4 mb-3">
          <div class="box p-5">
            <i class="fas fa-mouse fa-3x mb-4"></i>
            <h4>Web Design</h4>
            <p>
              Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
              Sed id mauris vel neque
            </p>
            <a class="readmore" href="#"><span>Read More</span></a>
          </div>
        </div>
        <div class="col-md-6 col-lg-4 mb-3">
          <div class="box p-5">
            <i class="fas fa-camera-retro fa-3x mb-4"></i>
            <h4>Photography</h4>
            <p>
              Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
              Sed id mauris vel neque
            </p>
            <a class="readmore" href="#"><span>Read More</span></a>
          </div>
        </div>
        <div class="col-md-6 col-lg-4 mb-3">
          <div class="box p-5">
            <i class="fab fa-youtube fa-3x mb-4"></i>
            <h4>Video Editing</h4>
            <p>
              Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
              Sed id mauris vel neque
            </p>
            <a class="readmore" href="#"><span>Read More</span></a>
          </div>
        </div>
        <div class="col-md-6 col-lg-4 mb-3">
          <div class="box p-5">
            <i class="fas fa-pencil-alt fa-3x mb-4"></i>
            <h4>Writing</h4>
            <p>
              Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
              Sed id mauris vel neque
            </p>
            <a class="readmore" href="#"><span>Read More</span></a>
          </div>
        </div>
        <div class="col-md-6 col-lg-4 mb-3">
          <div class="box p-5">
            <i class="fas fa-laptop-code fa-3x mb-4"></i>
            <h4>Coding</h4>
            <p>
              Duis molestie enim mattis gravida viverra. Fusce ut eros augue.
              Sed id mauris vel neque
            </p>
            <a class="readmore" href="#"><span>Read More</span></a>
          </div>
        </div>
        <div class="col-md-6 col-lg-4 mb-3">
          <div class="box p-5">
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
</template>

<script>
export default {};
</script>

<style>
.skills .box {
  background-color: #12141c;
  overflow: hidden;
  transition: 0.3s ease;
}
.skills .box i {
  color: #e9621eec;
  transition: inherit;
  transition-delay: 0s;
}
.skills h4 {
  color: #fff;
  transition: inherit;
  transition-delay: 0.05s;
}
.skills p {
  color: #dfdfdf;
  transition: inherit;
  transition-delay: 0.1s;
}
.readmore {
  color: #fff;
  overflow: hidden;
  display: inline-block;
  font-size: 0.75rem;
  text-transform: uppercase;
  font-weight: 700;
  color: #fff;
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