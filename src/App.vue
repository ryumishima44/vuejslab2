<template lang='pug'>
  #app
    search
</template>
<script>
import Search from './components/search/Search.vue'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Registro estación Platzi'
    }
  },
  components: {
    Search
  }
}
</script>
<style lang='scss'>
@import './scss/main.scss';

#app {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
