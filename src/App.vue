<template>
  <div>
    <h1>Rick and Morty</h1>
    <FilterByStatus />
    <FilterByName />
    <ListCharacters />
  </div>
</template>

<script>
import ListCharacters from '@/components/ListCharacters.vue';
import FilterByStatus from '@/components/FilterByStatus.vue';
import FilterByName from '@/components/FilterByName.vue';
export default {
  name: 'App',
  components: {
    ListCharacters,
    FilterByStatus,
    FilterByName
  }
}
</script>

<style lang="scss">
:root{
  --background-body: #24282F;
  --background-card: #3C3E44;
  --text-gray: #c0c0c0;
  --text-orange: #ff9800;
  --text-white: #fff;
}
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body {
  background-color: var(--background-body);
  color: var(--text-white);
  font-family: 'Roboto', sans-serif;
}
h1 {
  margin-bottom: 3rem;
  text-align: center;
}
.container {
  max-width: 90%;
  width: 980px;
  margin: 5rem auto;
}
img {
  width: 100%;
}
</style>
