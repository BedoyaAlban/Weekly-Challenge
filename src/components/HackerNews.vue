<template>
  <h1>Hacker News</h1>
</template>

<script>
export default {
  setup() {
    async function getResults() {
      const url = "http://hn.algolia.com/api/v1/search?query=front_page";
      const response = await fetch(url, {
        headers: {
          accept: "application/json"
        }
      });
      const data = await response.json();
      console.log(data.hits);
    }

    getResults();
  }
};
</script>