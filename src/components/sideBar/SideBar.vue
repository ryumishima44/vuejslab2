<template lang='pug'>
  #sidebar
    div.sidebar-container
      div.sidebar-container__card
        img(src='../../assets/home.svg')
        p Home
      div.sidebar-container__card
        img(src='../../assets/claqueta.svg')
        p Trending
      div.sidebar-container__card
        img(src='../../assets/like.svg')
        p Most Liked
      div.sidebar-container__card#settings
        img(src='../../assets/setting.svg')
        p Settings
</template>
<script>
export default {
  name: 'sidebar',
  data () {
    return {
    }
  }
}
</script>
<style lang='scss'>
.sidebar-container {
  display: flex;
  flex-direction: column;
  position: absolute;
  align-items: center;
  left: 0;
  width: 89px;
  height: 100vh;
  background-image: linear-gradient(#ff535b,#fd746c)
}

.sidebar-container__card {
  color: #fff;
  text-align: center;
  margin: 20px 0 30px;
  cursor: pointer;
  &#settings {
    position: absolute;
    bottom: 0;
  }
}
</style>
