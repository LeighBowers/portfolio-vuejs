<template>
  <!-- education -->
  <section id="resume">
    <div class="edu">
      <div class="res-title"><h1>Resume</h1></div>
      <div class="container">
        <div class="row text-center">
          <div class="col">
            <div class="edu-container">
              <div class="header">
                <span class="name">Education</span>
              </div>
              <div class="content">
                <div class="info">
                  <!-- <span class="dark-bg">2021</span>

                  <h6>Web Development</h6>
                  <p>Life Choices</p>
                  <hr /> -->
                  <span class="dark-bg">July 2014-March 2015</span>
                  <h6>Social Auxiliary Work Student</h6>
                  <p>Hugenote College</p>
                  <hr />
                  <span class="theme-bg">2011</span>
                  <h6>Grade 12</h6>
                  <p>Modderdam High School</p>
                  <hr />
                </div>
              </div>
            </div>
          </div>

          <div class="col">
            <div class="edu-container">
              <div class="header">
                <span class="name">Experience</span>
              </div>
              <div class="content">
                <div class="info">
                  <!-- <span class="dark-bg">September 2021</span>

                  <h6>Life Choices Academy</h6>
                  <p>
                    Learning Modern Web Languages like HTML, CSS, JavaScrip &
                    Front End Frameworks.
                  </p>
                  <hr /> -->
                  <span class="dark-bg">1 June 2019-June 2017</span>
                  <h6>STEP BY STEP EDUCARE</h6>
                  <p>POSITION HELD: Teachers / Intern</p>
                  <hr />
                  <span class="theme-bg">1 April 2018-15 March 2019</span>
                  <h6><span class="title">BOUNDARY PRIMARY SCHOOL</span></h6>
                  <p>
                    POSITION HELD: Teachers assistant/Government Supporting
                    Program/Intern
                  </p>
                  <hr />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <br />

    <!-- bar -->
    <div class="container">
      <div class="row">
        <div class="col">
          <img src="https://i.postimg.cc/25FwD6cy/desk.jpg" alt="" />
        </div>
        <div class="col">
          <div class="container-skills">
            <div class="html">
              <p class="bar-title">
                HTML
                <span class="percent align-right">90%</span>
              </p>
              <div class="bar">
                <div class="bar-fill bar-fill-html start"></div>
              </div>
            </div>
            <div class="css">
              <p class="bar-title">
                CSS
                <span class="percent align-right">60%</span>
              </p>
              <div class="bar">
                <div class="bar-fill bar-fill-css start"></div>
              </div>
            </div>
            <div class="javascript">
              <p class="bar-title">
                Javascript
                <span class="percent align-right">70%</span>
              </p>
              <div class="bar">
                <div class="bar-fill bar-fill-javascript start"></div>
              </div>
            </div>
            <div class="bootstrap">
              <p class="bar-title">
                Bootstrap
                <span class="percent align-right">90%</span>
              </p>
              <div class="bar">
                <div class="bar-fill bar-fill-bootstrap start"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- skills -->
    <section id="skills">
      <div class="skill-title"><h1>Skills</h1></div>

      <main>
        <div class="grid">
          <div class="box">
            <div class="inner-box">
              <i class="fas fa-mouse fa-3x mb-4"></i>
              <h4>Web Design</h4>
              <p>
                Prepares content for the Web. This role is mainly related to the
                styling and layout of pages with content, including text and
                images. Web designers use many technologies but commonly rely on
                hypertext and hypermedia resources including HTML, CSS and
                additional Web design tools.
              </p>
            </div>
          </div>

          <div class="box">
            <div class="inner-box">
              <i class="fas fa-laptop-code fa-3x mb-4"></i>
              <h4>Coding</h4>
              <p>
                Designing instructions between the language we speak, and the
                language a computer understands.writing script for a computer
                program or mobile device.
              </p>
            </div>
          </div>

          <div class="box">
            <div class="inner-box">
              <i class="fas fa-mobile-alt fa-3x mb-4"></i>
              <h4>App Developing</h4>
              <p>
                Creating a computer program or a set of programs to perform the
                different tasks that is requires.
              </p>
            </div>
          </div>

          <div class="box">
            <div class="inner-box">
              <i class="fas fa-mouse fa-3x mb-4"></i>
              <h4>Web Development</h4>
              <p>
                Work in developing a website for the Internet (World Wide
                Web).Building and maintenance of websites.Work that happens
                behind the scenes to make a website look great, work fast and
                perform well with a seamless user experience.
              </p>
            </div>
          </div>
        </div>
      </main>
    </section>
  </section>
</template>

<script>
export default {};
</script>

<style>
/* experience */
.resume {
  margin-top: 20%;
  width: 100%;
}
.res-title {
  position: relative;
  padding-bottom: 2px;
}
.res-title {
  position: relative;
  color: #e9621eec;
  font-size: 18px;
  font-weight: 700;
  padding-right: 50px;
  margin-bottom: 15px;
  display: inline-block;
  text-transform: capitalize;
}
.res-title :before {
  position: absolute;
  content: "";
  right: 0px;
  bottom: 7px;
  width: 40px;
  height: 1px;
  background-color: #e9621eec;
}

.edu-container {
  background: #fff none repeat scroll 0% 0%;
  box-shadow: 0px 1px 3px rgba(0, 0, 0, 0.2);
}
.edu-container .header {
  padding: 5px;
  border-top: 5px solid #e9621eec;
  border-bottom: 1px solid #ddd;
}

.edu-container .header .name {
  display: block;
  font-size: 18px;
  color: rgb(24, 23, 23);
}

.edu-container.header .position {
  display: block;
}

.edu-container .content {
  position: relative;
}

.edu-container .content .info {
  padding: 10px;
  text-align: left;
  width: 100%;
}

/* bar */
.container-skills {
  margin: 20px auto 0 auto;
  max-width: 500px;
}

.bar {
  position: relative;
  background-color: #d8d8d8;
  height: 10px;
  margin: 0 0 20px 0;
}
.bar-fill {
  position: absolute;
  height: 10px;
}
.bar-title {
  position: relative;
  font-size: 1em;
  text-align: left;
  margin: 0 0 5px 0;
}
.percent {
  position: absolute;
  right: 0;
}

/* Animations Below - Replace ease-out with infinite for infinite loop*/
/*Edit here for html*/
.bar-fill-html {
  width: 90%;
  background-color: #e9621eec;
  animation: bar-fill-html 2s ease-out;
  -moz-animation: bar-fill-html 2s ease-out;
  -webkit-animation: bar-fill-html 2s ease-out;
}
@keyframes bar-fill-html {
  0% {
    width: 0px;
  }

  100% {
    width: 90%;
  }
}
@-moz-keyframes bar-fill-html {
  0% {
    width: 0px;
  }

  100% {
    width: 90%;
  }
}
@-webkit-keyframes bar-fill-html {
  0% {
    width: 0px;
  }

  100% {
    width: 90%;
  }
}
/*Edit here for Javascript*/
.bar-fill-css {
  width: 60%;
  background-color: #e9621eec;
  animation: bar-fill-css 2s ease-out;
  -moz-animation: bar-fill-css 2s ease-out;
  -webkit-animation: bar-fill-css 2s ease-out;
}
@keyframes bar-fill-css {
  0% {
    width: 0px;
  }

  100% {
    width: 60%;
  }
}
@-moz-keyframes bar-fill-css {
  0% {
    width: 0px;
  }

  100% {
    width: 60%;
  }
}
@-webkit-keyframes bar-fill-css {
  0% {
    width: 0px;
  }

  100% {
    width: 60%;
  }
}
/* end */
.bar-fill-javascript {
  width: 70%;
  background-color: #e9621eec;
  animation: bar-fill-javascript 2s ease-out;
  -moz-animation: bar-fill-javascrip 2s ease-out;
  -webkit-animation: bar-fill-javascript 2s ease-out;
}
@keyframes bar-fill-javascript {
  0% {
    width: 0px;
  }

  100% {
    width: 70%;
  }
}
@-moz-keyframes bar-fill-javascript {
  0% {
    width: 0px;
  }

  100% {
    width: 70%;
  }
}
@-webkit-keyframes bar-fill-javascript {
  0% {
    width: 0px;
  }

  100% {
    width: 70%;
  }
}
.bar-fill-bootstrap {
  width: 70%;
  background-color: #e9621eec;
  animation: bar-fill-bootstrap 2s ease-out;
  -moz-animation: bar-fill-botstrap 2s ease-out;
  -webkit-animation: bar-fill-bootstrap 2s ease-out;
}
@keyframes bar-fill-bootstrap {
  0% {
    width: 0px;
  }

  100% {
    width: 70%;
  }
}
@-moz-keyframes bar-fill-bootstrap {
  0% {
    width: 0px;
  }

  100% {
    width: 70%;
  }
}
@-webkit-keyframes bar-fill-bootstrap {
  0% {
    width: 0px;
  }

  100% {
    width: 70%;
  }
}

/* skills */
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
  margin-bottom: 5px;
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
  background-color: #e9621eec;
}
main {
  margin: 5em 5em;
}

@media screen and (max-width: 600px) {
  main {
    margin: 0.4em;
  }
}

#container {
  margin: 0 1em;
  padding: 3em;
  border-radius: 3px;
  border: 1px solid #e9621eec;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.9);
}

@media screen and (max-width: 600px) {
  #container {
    font-size: 1em;
    padding: 0.6em;
  }
}

.grid {
  margin: 5em auto;
  padding: 0 1em;
  max-width: 100%;
  display: grid;
  grid-auto-rows: max-content;
  grid-template-columns: repeat(auto-fit, minmax(14em, 1fr));
  grid-gap: 1em;
}

.box {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.6);
  padding: 2em;
  text-align: center;
  color: #080808;
  background: linear-gradient(45deg, #d6926b, #ddf0b2, #dfa576);
  border-radius: 3px;
  border: 2px solid rgba(56, 54, 56, 0.644);
  opacity: 0.8;
}

.box:hover {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.9);
  border: 2px solid rgb(212, 121, 16);
  opacity: 1;
}
</style>