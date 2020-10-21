<template>
  <PRSearch />
</template>

<script>
import PRSearch from './features/PRSearch';

export default {
  name: 'App',
  components: {
    PRSearch,
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

