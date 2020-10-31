<template>
<!-- TODO Create a section with the title, a short (1-2 sentence) mention of what this site is,  -->
<h1> Welcome to PR Practice </h1>
<p> Need something to review? Click the button to get a random PR to look at, if you want language specific, select some languages below. </p>
  <PRSearch />
  <LanguageSelection />
</template>

<script>
import PRSearch from './features/PRSearch';
import LanguageSelection from './features/LanguageSelection';

export default {
  name: 'App',
  components: {
    PRSearch,
    LanguageSelection,
  }
}
</script>

<style>
@import url('./colors.css');
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: var(--primary);
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-content: center;
}
</style>

