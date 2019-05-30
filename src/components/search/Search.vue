<template lang='pug'>
  #search
    div.search-container
      img.logo(src='../../assets/movie.jpg')
      input.search-box(type='text' placeholder='Search for your favorite movies')
      div.user-container
        p Francisco Sanchez
        img.user-pic(src='../../assets/avatar.png')
        i.arrow
</template>
<script>
export default {
  name: 'search',
  data () {
    return {
    }
  }
}
</script>
<style lang='scss'>
#search {
  width: 100%;
  box-shadow: 0px 1px 15px -5px;
}

.search-container {
  display: flex;
  height: 60px;
  align-items: center;
  justify-content: center;

  .logo {
    position: absolute;
    left: 0;
    margin-left: 20px;
  }

  .search-box {
    font-size: 14px;
    width: 30%;
    padding: 10px;
    border-radius: 5px;
    border-style: solid;
    border: 1px solid #bbb;

  }

  .user-container {
    position: absolute;
    right: 0;
    margin-right: 20px;
    display: flex;
    align-items: center;

    p {
      padding-right: 10px;
    }
    .user-pic {
      border-radius: 20px;
      margin-right: 10px;
      width: 40px;
      height: 40px;
    }
    .arrow {
      border: solid black;
      border-width: 0 3px 3px 0;
      display: inline-block;
      padding: 3px;
      transform: rotate(45deg);
    }
  }
}
</style>
