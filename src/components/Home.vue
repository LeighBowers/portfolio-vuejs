<template>
  <div class="home">
    <h2 class="heading">Hi there, Im</h2>
    <h1 class="heading">Leigh-Anne Bowers</h1>
    <span id="text"><h3>Aspired</h3></span>
  </div>
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
  await writeWord("Aspired Web Designer");
  await waitForMs(1500);
  await deleteWord();
  await waitForMs(500);
  await writeWord("Im a Student at Life Choices Academy");
  await waitForMs(1500);
  await deleteWord();
  await waitForMs(500);
  await writeWord("Work hard Play even harder");
  await waitForMs(1500);
  await deleteWord();
  await waitForMs(500);
  await writeWord("LOVE");
}

typingEffect();
</script>


<style>
.home {
  background-image: url("https://i.postimg.cc/1Xcjts64/Leigh-ann3.jpg");
  background-position: cover;
  background-size: cover;
  height: 100vh;
}

h1.heading {
  font-size: 4rem;

  padding-top: 30px;
}
h2.heading {
  font-size: 4rem;

  padding-top: 10%;
}
h3 {
  font-size: 4rem;

  padding-top: 30px;
}
</style>