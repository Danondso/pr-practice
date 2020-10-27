<template>
  <div class="language-selection-container">
      <div class="language-selection-item-wrapper" v-bind:key="language" v-for="(language) in languages">
        <Pill v-bind:text="language.name" v-bind:color="language.color" v-bind:onClick="onClick" />
      </div>
  </div>
</template>

<script>
// https://github.com/github/linguist/blob/master/lib/linguist/languages.yml use this to get all languages
// parse the yml file and shove them into an array and generate the pills for it
// create a all-languages selection that when clicked, give you ALL the pills to look at

// For starters, we'll use the top ten most active according to this site: https://learnworthy.net/10-most-active-programming-languages-in-github/
import Pill from "../components/Pill.vue";
import { DEFAULT_LANGUAGES } from '../constants/defaultLanguages.js';
export default {
  name: "LanguageSelection",
  props: {
    searchText: String,
  },
  components: {
    Pill,
  },
  data() {
    return {
        languages: DEFAULT_LANGUAGES,
        onClick: (text) => { console.log(text);} // TODO push the selected language to the selected languages bit of state and change the colour
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.language-selection-container {
  flex-flow: row wrap;
}
.language-selection-item-wrapper {
  display: inline-block;
  padding: 0 0.75rem 0 0.75rem;
}
</style>
