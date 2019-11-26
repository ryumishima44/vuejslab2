<template lang='pug'>
  #app
    section.section
      nav.nav.has-shadow
        .container
          input.input.is-large(type="text",
                               placeholder="Buscar canciones",
                               v-model='query')
          a.button.is-info.is-large(@click="search") Buscar
          a.button.is-danger.is-large &times;

        .container {{ searchMsg }}
          .columns
            .column(v-for="track in tracks") {{ track.name }} - {{ track.artist }}
</template>
<script>
const tracks = [
  {
    name: 'Muchacha',
    artist: 'Spindola'
  },
  {
    name: 'Chaule',
    artist: 'Prajakta'
  },
  {
    name: 'Aguas wey',
    artist: 'Tropikal forever'
  }
]
export default {
  name: 'App',

  data () {
    return {
      query: '',
      tracks: []
    }
  },
  computed: {
    searchMsg () {
      return `${this.tracks.length} Resultados`
    }
  },
  methods: {
    search () {
      this.tracks = tracks
    }
  }
}
</script>
<style lang='scss'>
@import './scss/main.scss';
</style>
