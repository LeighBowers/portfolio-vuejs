<template>
  <section id="about">
    <div class="about-section">
      <div class="container">
        <div class="row clearfix">
          <!--Image Column-->
          <div class="image-column col-md-6">
            <div
              class="inner-column"
              data-wow-delay="0ms"
              data-wow-duration="1500ms"
            >
              <div class="image">
                <img
                  src="https://i.postimg.cc/1Xcjts64/Leigh-ann3.jpg"
                  alt=""
                />
                <div class="overlay-box"></div>
              </div>
            </div>
          </div>
          <!--Content Column-->
          <div class="content-column col-md-6">
            <div class="inner-column">
              <div class="sec-title">
                <div class="about-text">
                  <div class="title"><h1>About Me</h1></div>
                  <h2>Aspired <br /></h2>

                  I am a hard-working, passionate individual who loves to learn
                  nnew things. Although I am a soft talker, I can hold my own
                  when required. I am friendly and easy to talk to and work well
                  in a team.
                </div>
              </div>
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
.about-section {
  background: linear-gradient(to bottom, rgba(245, 246, 252, 0.356), #e9621e83),
    url("");
  /* background-position: cover; */
  background-size: cover;
  height: 100vh;
}
.about-section {
  /* position: relative; */
  padding: 120px 0px;
}

.about-section .content-column {
  position: relative;
  margin-bottom: 40px;
}

.about-section .content-column .inner-column {
  position: relative;
  padding-top: 50px;
  padding-right: 100px;
}

.about-section .content-column .text {
  position: relative;
  color: #777777;
  font-size: 15px;
  line-height: 2em;
  margin-bottom: 40px;
}

.about-section .image-column .inner-column {
  position: relative;
  padding: 40px 100px 20px 0px;
  margin-left: -10px;
}

.about-section .image-column .inner-column:after {
  position: absolute;
  content: "";
  right: 0px;
  top: 0px;
  left: 40px;
  bottom: 100px;

  z-index: -1;
  border: 2px solid #e9621eec;
}

.about-section .image-column .inner-column .image img {
  position: relative;
  width: 100%;

  /* display: block; */
}

.about-section .btn-style-three:before {
  position: absolute;
  content: "";
  left: 10px;
  top: 10px;
  z-index: -1;
  right: -10px;
  bottom: -10px;
  /* background: url(https://i.ibb.co/DKn55Qz/pattern-1.jpg) repeat; */
}
.about-section .btn-style-three:hover {
  color: #ffffff;
  background: #e9621eec;
}
.about-section .btn-style-three {
  position: relative;
  line-height: 24px;
  color: #252525;
  font-size: 15px;
  font-weight: 700;
  background: none;
  /* display: inline-block; */
  padding: 11px 40px;
  background-color: #ffffff;
  text-transform: capitalize;
  border: 2px solid #e9621eec;
  font-family: "Arimo", sans-serif;
}

.about-text {
  padding-bottom: 20%;
}

.sec-title2 {
  color: #fff;
}
.sec-title {
  position: relative;
  padding-bottom: 40px;
}
.sec-title .title {
  position: relative;
  color: #e9621eec;
  font-size: 18px;
  font-weight: 700;
  padding-right: 50px;
  margin-bottom: 15px;
  display: inline-block;
  text-transform: capitalize;
}
.sec-title .title:before {
  position: absolute;
  content: "";
  right: 0px;
  bottom: 7px;
  width: 40px;
  height: 1px;
  background-color: #d66e28;
}
/* experience */
</style>