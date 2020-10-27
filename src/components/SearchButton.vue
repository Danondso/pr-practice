<template>
  <button class="searchButton"><h1>{{ searchButtonText }}</h1></button>
</template>

<script>
export default {
  name: "SearchButton",
  props: {
    searchButtonText: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('../colors.css');
button, input[type="submit"], input[type="reset"] {
  border: #000000;
  background: none;
	color: inherit;
	border: none;
	padding: 0;
	font: inherit;
	cursor: pointer;
	outline: inherit;
  font-size: 1rem;
  transition: 1s;
  border-radius: 40px;
  border-width: 2px;
  padding: 0.05rem;
}
button:hover {
  background-color: var(--secondary);
  color: var(--primary-background);
}
</style>
