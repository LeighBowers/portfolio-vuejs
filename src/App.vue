<template>
  <Navbar />
  <Home />
  <About />
  <Resume />
  <Projects />
  <Testimonials />
  <Contact />

  <!-- <Sections /> -->
</template>
<script>
import Navbar from "@/components/Navbar.vue";
import Home from "@/components/Home.vue";
import About from "@/components/About.vue";
import Resume from "@/components/Resume.vue";
import Projects from "@/components/Projects.vue";
import Testimonials from "@/components/Testimonials.vue";
import Contact from "@/components/Contact.vue";

// import Sections from "components/Sections.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Home,
    About,
    Projects,
    Testimonials,
    Contact,
    Resume,
  },
};
</script>
<style>
#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  font-size: 20px;
  text-decoration: none;
  padding: 10px;
  border-radius: 4px;
}

#nav a.router-link-exact-active {
  color: #d2e2db;
  background: #d42929;
}
</style>