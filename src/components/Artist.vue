<template lang="pug">
  li.artist
    h2: a(:href="artist.url" target="_blank") {{ artist.name }}
    img(:src="artist.image[2]['#text']")
</template>

<script>
export default {
  //   Definimos el nombre del component definido en vue.js
  name: 'artist',
  //  Definimos la propiedad que recibe el component, en :bind en vue.js
  props: [ 'artist' ]
}
</script>

<style lang="stylus" scoped>
li.artist
  display block
  margin 10px 0
</style>



