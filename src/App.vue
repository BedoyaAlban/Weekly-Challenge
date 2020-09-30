<template>
  <div>
    <NavBar />
    <HackerNews />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import HackerNews from "./components/HackerNews.vue";

export default {
  name: "App",
  components: {
    NavBar,
    HackerNews
  }
};
</script>


