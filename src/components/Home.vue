<template>
  <section id="home">
    <div class="home">
      <h2>Hi there, I`m</h2>
      <h1>Leigh-Anne Bowers</h1>
      <span id="text"></span>
    </div>
  </section>
</template>

<script>
//Function to force a waiting period
function waitForMs(ms) {
  return new Promise((resolve) => setTimeout(resolve, ms));
}
async function deleteWord() {
  let sentence = document.querySelector("#text").innerHTML.trim();
  console.log(sentence);

  let characters = sentence.split("");
  console.log(characters);

  while (characters.length > 0) {
    await waitForMs(100);
    characters.pop();
    document.querySelector("#text").innerHTML = characters.join("");
  }
}

async function writeWord(word) {
  let character = word.split("");
  console.log(character);

  let i = 0;
  while (i < character.length) {
    await waitForMs(100);
    document.querySelector("#text").append(character[i]);
    i++;
  }
}

async function typingEffect() {
  await deleteWord();
  await waitForMs(500);
  await writeWord("Aspired Web Developer");
  await waitForMs(1500);
  await deleteWord();
  await waitForMs(500);
  await writeWord("Aspired Web Designer");
  await waitForMs(1500);
  await deleteWord();
  await waitForMs(500);
  await writeWord("");
  await waitForMs(1500);
  await deleteWord();
  await waitForMs(500);
}

typingEffect();
</script>


<style>
#text {
  position: absolute;
  text-align: center;
  left: 0;
  width: 100%;
}
.home {
  /* background-image: ("https://i.postimg.cc/7hrVCmVP/new-back.jpg");
  background: linear-gradient(blue, pink); */
  background-image: linear-gradient(
      to bottom,
      rgba(245, 246, 252, 0.356),
      #e9621e83
    ),
    url("https://i.postimg.cc/5y69kVdt/developback.jpg");
  background-position: cover;
  background-size: cover;
  height: 100vh;
}

h2 {
  font-size: 4rem;

  padding-top: 20%;
}
</style>