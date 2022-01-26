<template>
  <section id="contact">
    <div class="row justify-content-center my-5">
      <div class="contact head text-center col-lg-6">
        <h2>Get in Touch</h2>
        <p class="lead">
          Questions to ask? Fill out the form to contact me directly...
        </p>
      </div>
    </div>

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
            <div class="icons"><i class="bi bi-envelope-open"></i></div>
            <h4>Email</h4>
            <p>leighbowers@gmail.com</p>
          </div>
        </div>
      </div>
    </div>
    <form
      class="contact-sub col-lg-6"
      action="https://formspree.io/f/xjvjqbag"
      target="_blank"
      method="post"
    >
      <label for="name" class="form-label">Name:</label>
      <div class="mb-4 input-group">
        <span class="input-group-text">
          <i class="bi bi-person-fill text-secondary"></i>
        </span>
        <input name="name" type="text" class="form-control" placeholder="" />
      </div>

      <label for="email" class="form-label">Email address:</label>
      <div class="input-group mb-4">
        <span class="input-group-text">
          <i class="bi bi-envelope-fill text-secondary"></i>
        </span>
        <input name="email" type="email" class="form-control" placeholder="" />
      </div>

      <div class="mb-4 mt-5 form-floating">
        <textarea
          name="query"
          class="form-control"
          id="query"
          style="height: 140px"
          placeholder="query"
        ></textarea>
        <label for="query">Your Message</label>
      </div>

      <button type="submit" class="btn btn-dark">Submit</button>
    </form>

    <!-- Modal -->

    <!-- Foot -->
    <div class="footer-basic">
      <footer>
        <div class="social">
          <a href="https://github.com/LeighBowers/Project1" target="_blank"
            ><i class="bi bi-github"></i
          ></a>

          <a
            href="https://www.linkedin.com/public-profile/settings?trk=d_flagship3_profile_self_view_public_profile&lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_self_edit_contact_info%3Bc58V4dWYQ7GIbDRqcFsLjw%3D%3D"
            target="_blank"
            ><i class="bi bi-linkedin"></i
          ></a>

          <a
            href="https://app.netlify.com/sites/leigh-anne-portfolio/settings/general"
            target="_blank"
            ><i class="bi bi-grid-fill"></i
          ></a>
        </div>
        <ul class="list-inline">
          <li class="list-inline-item"><a href="#">Home</a></li>
          <li class="list-inline-item"><a href="#projects">Projects</a></li>
          <li class="list-inline-item"><a href="#about">About</a></li>
          <li class="list-inline-item"><a href="#">Terms</a></li>
          <li class="list-inline-item"><a href="#">Privacy Policy</a></li>
        </ul>
        <p class="copyright">Company Name © 2018</p>
      </footer>
    </div>
  </section>
</template>
            
<script>
export default {};
</script>

<style>
</style>