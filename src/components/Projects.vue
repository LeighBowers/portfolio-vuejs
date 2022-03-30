<template>
  <section id="projects">
    <div class="pr-title"><h1>Projects</h1></div>
    <main>
      <div class="grid">
        <div v-for="project in projects" :key="project.id" class="section">
          <img class="card-img-top" :src="project.img" alt="..." />

          <h2>{{ project.title }}</h2>

          <button type="submit" class="btn">
            <a :href="project.netlify" target="_blank">Netlify</a>
            <!-- <br /> -->
          </button>
          <button type="submit" class="btn">
            <a :href="project.github" target="_blank">Github </a>
          </button>
        </div>
      </div>
    </main>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [],
    };
  },
  mounted() {
    fetch("https://leigh-anne-api.herokuapp.com/projects")
      .then((res) => res.json())
      .then((data) => (this.projects = data))
      .catch((err) => console.log(err.message));
  },
};
</script>
<style>
.pr-title {
  position: relative;
  padding-bottom: 2px;
}
.pr-title {
  position: relative;
  color: #12777eec;
  font-size: 18px;
  font-weight: 700;
  padding-right: 50px;
  margin-bottom: 15px;
  display: inline-block;
  text-transform: capitalize;
}
.pr-title :before {
  position: absolute;
  content: "";
  right: 0px;
  bottom: 5px;
  width: 40px;
  height: 1px;
  background-color: #12777eec;
}

main {
  margin: 2em 3em;
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
  border: 1px solid rgba(156, 175, 172, 0.7);
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.9);
}

@media screen and (max-width: 600px) {
  #container {
    font-size: 1em;
    padding: 0.6em;
  }
}
#projects {
  margin-top: -200px;
}
.grid {
  margin: 5em auto;
  padding: 0 1em;
  max-width: 100%;
  display: grid;
  grid-template-columns: repeat(3, 200px);
  grid-template-columns: 200px 200px 200px;
  /* grid-auto-rows: max-content; */
  grid-template-columns: repeat(auto-fit, minmax(14em, 1fr));
  grid-gap: 1em;
}

.section {
  box-shadow: 0 4px 8px 0 rgba(170, 158, 158, 0.6);
  padding: 2em;
  text-align: center;
  color: #080808;
  background: linear-gradient(45deg, #a8b1c4, #d3cbc78c);
  border-radius: 3px;
  border: 2px solid rgba(77, 95, 201, 0.7);
  opacity: 0.8;
}

.section:hover {
  box-shadow: 0 4px 8px 0 rgba(27, 31, 97, 0.9);
  border: 2px solid rgb(190, 186, 179);
  opacity: 1;
}

.section button {
  border: none;
  outline: 0;
  padding: 12px;
  color: white;
  background-image: linear-gradient(to right, #f7e7e0, #64a9c4);
  text-align: center;
  cursor: pointer;
  width: 100%;
  font-size: 1em;
  border-radius: 2px;
}

.section button:hover {
  background-color: rgb(136, 124, 109);
  background-image: linear-gradient(to left, #9c948a, #526692);
}
</style>
