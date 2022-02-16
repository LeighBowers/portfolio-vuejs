<template>
  <section id="home">
    <div class="home">
      <h1>Leigh-Anne Bowers</h1>
      <h1>Aspired</h1>
      <div class="typing-slider">
        <p>Web Developer</p>
        <p>Web Designer</p>
        <p>Full-Stack Developer</p>
      </div>
      <!-- <span id="text"></span> -->
    </div>
  </section>
</template>

<script>
</script>


<style>
.home {
  padding-top: 10%;
}
#text {
  position: absolute;
  text-align: center;
  left: 0;
  width: 100%;
  font-size: 50px;
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

@keyframes cursor {
  from,
  to {
    border-color: transparent;
  }
  50% {
    border-color: rgb(179, 96, 71);
  }
}
@keyframes typing {
  from {
    width: 100%;
  }
  90%,
  to {
    width: 0;
  }
}
@keyframes slide {
  33.3333333333% {
    font-size: 3rem;
    letter-spacing: 3px;
  }
  to {
    font-size: 0;
    letter-spacing: 0;
  }
}
.typing-slider {
  font-family: Consolas, monospace;
  font-weight: bold;
  text-align: center;
  white-space: nowrap;
}

.typing-slider p {
  position: relative;
  display: inline;
  font-size: 0;
  text-transform: uppercase;
  letter-spacing: 0;
  animation: slide 15s step-start infinite;
}

.typing-slider p::after {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  border-left: 3px solid black;
  background-color: rgba(129, 96, 69, 0.76);
  animation: typing 5s infinite, cursor 1s infinite;
}

.typing-slider p:nth-child(1) {
  animation-delay: 0s;
}
.typing-slider p:nth-child(1)::after {
  animation-delay: 0s;
  animation-timing-function: steps(16), step-end;
}

.typing-slider p:nth-child(2) {
  animation-delay: 5s;
}
.typing-slider p:nth-child(2)::after {
  animation-delay: 5s;
  animation-timing-function: steps(23), step-end;
}

.typing-slider p:nth-child(3) {
  animation-delay: 10s;
}
.typing-slider p:nth-child(3)::after {
  animation-delay: 10s;
  animation-timing-function: steps(12), step-end;
}
</style>