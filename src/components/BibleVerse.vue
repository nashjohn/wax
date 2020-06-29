<template>
  <transition
    name="intro"
    appear
    appear-active-class="intro-enter-active"
    appear-to-class="the-end"
    appear-class="the-show"
  >
    <div class="verse">
      <p class="paul">
        “Then Paul and Barnabas <span class="waxed"> waxed bold,</span> and
        said, It was necessary that the word of God should first have been
        spoken to you: but seeing ye put it from you, and judge yourselves
        unworthy of everlasting life,”
      </p>
    </div>
  </transition>
</template>

<script></script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped lang="scss">
.verse {
  background-color: black;
  color: white;
  height: 100vh;
  width: 100wh;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 100;
}
.waxed {
  color: yellow;
}
.paul {
  width: 50%;
  display: block;
  align-content: middle;
  line-height: 1.5em;
  font-size: 2.35em;
  letter-spacing: 0.05em;
  font-weight: 10;
  text-align: left;
  font-family: "Alegreya Sans", sans-serif;
  z-index: 100;
}
.paul {
  animation: simon 12s fowards;
}
@keyframes simon {
  0% {
    opacity: 1;
  }
  90% {
    opacity: 1;
  }
  95% {
    opacity: 0.5;
  }
  100% {
    opacity: 0;
  }
}
.verse {
  animation: in 5s forwards;
}
@keyframes in {
  0% {
    opacity: 0.5;
  }
  100% {
    opacity: 0;
    display: none;
  }
}
</style>
