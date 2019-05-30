<template lang='pug'>
  #app
    search
    sideBar
</template>
<script>
import Search from './components/search/Search.vue'
import SideBar from './components/sideBar/SideBar.vue'
export default {
  name: 'app',
  data () {
    return {
      msg: 'Registro estación Platzi'
    }
  },
  components: {
    Search,
    SideBar
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
