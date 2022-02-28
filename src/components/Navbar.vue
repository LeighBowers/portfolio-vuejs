
  <template>
  <nav class="nav nav-">
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
        <img src="https://img.icons8.com/ios/50/000000/l.png" />

        <img />
      </li>
      <li><a href="#home">|Home|</a></li>

      <li><a href="#about">|About Me|</a></li>

      <li><a href="#resume">|Resume|</a></li>

      <li><a href="#projects">|Projects|</a></li>

      <li><a href="#testimonials">|Testimonials|</a></li>

      <li><a href="#contact">|Contact Me|</a></li>
    </ul>
  </nav>
</template>


<script>
</script>

<style>
.nav {
  width: 100%;
  background-color: #796b6469;
  z-index: 1;
  position: fixed; /* Set the navbar to fixed position */
  letter-spacing: 2px;
}
.nav__toggle {
  position: absolute;
  cursor: pointer;
  margin: 2rem 1rem;
  right: 0;
}

.close,
input[type="checkbox"] {
  display: none;
  color: rgb(10, 10, 10);
}

.nav__menu {
  display: flex;
  flex-direction: column;
  gap: 6rem;
  align-items: center;
  margin: 0.4rem;
}

li {
  list-style: none;
  display: none;
  color: rgb(8, 7, 8);
}
li:first-child {
  margin-right: auto;
  display: block;
}
.nav__menu a {
  text-decoration: none;
  color: rgb(12, 12, 14);
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