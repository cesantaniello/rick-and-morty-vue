<template>
  <div class="character">
    <img :src="character.image" :alt="character.name">
    <div class="character__info">
      <h3>{{ character.name }}</h3>
      <div class="status">
        <span
          :class="
            character.status === 'Alive' ? 'alive' :
            character.status === 'Dead' ? 'dead' :
            'default'
          "
        ></span>
        <span>{{ character.status }} - {{ character.species }}</span>
      </div>
      <div class="origin">
        <span>Origin: {{ character.origin.name }}</span>
      </div>
      <div class="location">
        <span>Location: {{ character.location.name }}</span>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: ['character'],
}
</script>

<style>

</style>