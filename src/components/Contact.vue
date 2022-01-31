<template>
  <section id="contact">
    <!--    Contacts    -->
    <div class="contact-container">
      <div class="row">
        <div class="col-md-12">
          <div class="contact-title"><h2 class="text-center">CONTACTS</h2></div>
        </div>
      </div>
      <br />

      <div class="row">
        <div class="col-md-12">
          <div class="jumbotron">
            <div class="row">
              <div class="col-md-6">
                <div class="container">
                  <form
                    action="https://formspree.io/f/xjvjqbag"
                    target="_blank"
                    method="post"
                  >
                    <div class="form-group">
                      <label for="name">Name</label>
                      <input
                        type="text"
                        class="form-control"
                        id="name"
                        placeholder="Leigh-Anne"
                        required
                      />
                    </div>
                    <div class="form-group">
                      <label for="last-name">Last name</label>
                      <input
                        type="text"
                        class="form-control"
                        id="last-name"
                        placeholder="Bowers"
                        required
                      />
                    </div>
                    <div class="form-group">
                      <label for="email">Email</label>
                      <input
                        type="email"
                        class="form-control"
                        id="email"
                        placeholder="leighsylvester9@gmail.com"
                        required
                      />
                    </div>
                    <div class="form-group">
                      <label for="massage">Massage</label>
                      <textarea
                        class="form-control"
                        id="massage"
                        rows="3"
                        required
                      ></textarea>
                    </div>
                    <br />
                    <button type="submit" class="btn btn-white">Send</button>
                    <!-- <small>Sorry, form now is out of order.</small> -->
                  </form>
                </div>
              </div>
              <!--contact form-->
              <div class="col-md-6">
                <div class="contact-text text-center mb-3" style="margin: 70px">
                  <div class="row mb-4">
                    <div class="col-ms-3">
                      <div class="contact-info-items padd-15">
                        <div class="icons"><i class="bi bi-telephone"></i></div>
                        <h4>Contact me on</h4>
                        <p>+27 8875 4545</p>
                      </div>
                    </div>
                    <div class="col-ms-3">
                      <div class="contact-info-items padd-15">
                        <div class="icons"><i class="bi bi-house"></i></div>
                        <h4>Home</h4>
                        <p>Cape Town, South Africa</p>
                      </div>
                    </div>
                    <div class="col-ms-3">
                      <div class="contact-info-items padd-15">
                        <div class="icons">
                          <i class="bi bi-envelope-open"></i>
                        </div>
                        <h4>Email</h4>
                        <p>leighbowers@gmail.com</p>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!--jumbotron-->
        </div>
      </div>

      <!--   FOOTER   -->
      <footer>
        <div class="container">
          <div class="row">
            <div class="col-lg-12">
              <ul class="list-inline">
                <li class="footer-menu-divider">&sdot;</li>
                <li>
                  <a href="#about">About</a>
                </li>
                <li class="footer-menu-divider">&sdot;</li>
                <li>
                  <a href="#services">Services</a>
                </li>
                <li class="footer-menu-divider">&sdot;</li>
                <li>
                  <a href="#contact">Contact</a>
                </li>
                <li>&sdot;</li>
              </ul>
              <p class="copyright text-muted small">
                Copyright &copy; 2016. All Rights Reserved
              </p>
            </div>
          </div>
        </div>
      </footer>
    </div>
  </section>
</template>
            
<script>
export default {};
</script>

<style>
.contact-title {
  position: relative;
  padding-bottom: 40px;
}
.contact-title {
  position: relative;
  color: #e9621eec;
  font-size: 18px;
  font-weight: 700;
  padding-right: 50px;
  margin-bottom: 15px;
  display: inline-block;
  text-transform: capitalize;
}
.contact-title :before {
  position: absolute;
  content: "";
  right: 0px;
  bottom: 7px;
  width: 40px;
  height: 1px;
  background-color: #d66e28;
}
/* Footer */
.contact-container {
  background: linear-gradient(to bottom, rgba(245, 246, 252, 0.356), #e9621e83),
    url("");
  background-position: cover;
  background-size: cover;
  height: 100vh;
}
footer .jumbotron {
  padding: 2rem 2rem;
}

/* media queries */
@media (max-width: 850px) {
  .jumbotron-fluid img {
    width: 80%;
  }
}

@media (max-width: 767px) {
  .jumbotron-fluid {
    margin-top: 115px;
    text-align: center;
  }
  .jumbotron-vertical-middle {
    margin-top: -60px;
  }
  form button {
    margin-bottom: 30px;
  }
  .jumbotron-fluid img {
    width: 50%;
  }
}
@media (max-width: 575px) {
  .jumbotron-fluid {
    margin-top: 130px;
  }
  .display-3 {
    font-size: 40px;
    font-weight: bold;
  }
  .jumbotron-vertical-middle {
    margin-top: -30px;
  }
  .jumbotron-fluid img {
    width: 50%;
  }
}
@media (max-width: 441px) {
  .jumbotron {
    margin-top: 170px;
  }
}
@media (max-width: 330px) {
  .jumbotron {
    margin-top: 210px;
  }
}
footer {
  padding: 50px 0;
  background-color: #1c1c1c;
}

a {
  color: #e4dede;
}

p.copyright {
  margin: 15px 0 0;
}
</style>