
  <template>
  <nav class="nav">
    <input type="checkbox" id="nav__checkbox" class="nav__checkbox" />
    <label for="nav__checkbox" class="nav__toggle">
      <img
        src="https://img.icons8.com/material-outlined/30/000000/menu--v1.png"
        class="hamburger"
      />
      <img src="https://img.icons8.com/plumpy/30/000000/x.png" class="close" />
    </label>

    <ul class="nav__menu">
      <li>
        <a href="#">
          <li><a href="home">Home</a></li>
        </a>
      </li>
      <li><a href="home">Home</a></li>

      <li><a href="about">About Me</a></li>

      <li><a href="projects">Projects</a></li>

      <li><a href="skills">Skills</a></li>

      <li><a href="contact">Contact Me</a></li>
    </ul>
  </nav>
</template>


<script>
</script>

<style>
.nav {
  border-bottom: 1px solid rgb(236, 226, 226);
}
.nav__toggle {
  position: absolute;
  cursor: pointer;
  margin: 0rem 1rem;
  right: 0;
}

.close,
input[type="checkbox"] {
  display: none;
}
.hamburger {
  margin-top: 0.2rem;
}
.nav__menu {
  display: flex;
  flex-direction: column;
  gap: 7rem;
  align-items: center;
  margin: 1rem;
}
li {
  list-style: none;
  display: none;
  color: antiquewhite;
}
li:first-child {
  margin-right: auto;
  display: block;
}
.nav__menu a {
  text-decoration: none;
  color: rgb(8, 8, 95);
  font-size: 1rem;
}
#nav__checkbox:checked ~ ul.nav__menu li {
  display: block;
  margin: 0%;
  padding: 0%;
}
#nav__checkbox:checked ~ label.nav__toggle .hamburger {
  display: none;
  gap: 0;
}
#nav__checkbox:checked ~ label.nav__toggle .close {
  display: block;
}

@media only screen and (min-width: 768px) {
  .nav__toggle {
    display: none;
  }
  .nav__menu {
    flex-direction: row;
  }
  .nav__menu li {
    display: block;
    gap: 0;
  }
}
</style>