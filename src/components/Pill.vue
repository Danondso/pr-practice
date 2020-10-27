<template>
  <button type="button" v-on:click="onClick(text)" :style="{backgroundColor: color}" class="pill"><span class="pill-text">{{ text }}</span></button>
</template>

<script>
export default {
  name: "Pill",
  props: {
    text: String,
    onClick: Function,
    color: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button, input[type="submit"], input[type="reset"] {
	background: none;
	color: inherit;
	border: none;
	padding: 0;
	font: inherit;
	cursor: pointer;
	outline: inherit;
}
.pill-wrapper {
  padding: 0 0 0 0;
}
.pill {
    border: 2px solid;
    border-radius: 25px;
    padding: 0.5rem 1rem 0.5rem 1rem;
    /* color: orange; TODO make this color come from the palette */
}
.pill-text {
    font-size: 1rem;
}
</style>
