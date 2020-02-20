<template lang="html">
  <div v-if='country'>
    <h1>Some Country Facts</h1>
    <hr>
    <h2>{{ country.name }}</h2>
    <img :src="country.flag" height= 50px />
    <p>Population: {{ country.population }}</p>
    <p>Capital: {{ country.capital }}</p>
  </div>
</template>

<script>
export default {
  name: 'country-detail',
  props: ['country']
}
</script>

<style lang="css" scoped>
</style>
