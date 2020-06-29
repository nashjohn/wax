<template>
  <div class="homer">
    <BibleVerse></BibleVerse>
  </div>
</template>

<script>
// @ is an alias to /src
import BibleVerse from "@/components/BibleVerse.vue";
export default {
  name: "Home",
  components: {
    BibleVerse
  }
};
</script>

<style scoped>
.homer {
  width: 100vw;
  height: 100%;
  display: block;
  background-image: url("/images/today.jpg");
  background-size: cover;
}
</style>
