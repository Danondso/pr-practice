<template>
  <button class="searchButton">{{ searchText }}</button>
</template>

<script>
export default {
  name: "SearchButton",
  props: {
    searchText: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
button {
  border: none;
}
</style>
