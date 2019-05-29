<template lang='pug'>
  #app
    img.logo(src='./assets/satellite.jpg')
    div.form-container
      h1 {{ msg }}
      form
        label(for='name') Name
        input.form-input(type='text' id='name' name='name')
        label(for='lastname') Last Name
        input.form-input(type='text' id='lastname' name='lastname')
        label(for='role') Role
        input.form-input(type='text' id='role' name='role')
        input.form-submit(type='submit')
</template>
<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Registro estación Platzi'
    }
  }
}
</script>
<style lang='scss'>
@import './scss/main.scss';

#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 320px;
  max-height: 409px;
}

h1 {
  margin: 0 auto;
  font-weight: bold;
  color: #00BFD6;
}

.logo {
  margin: 10px 0;
}

.form-container {
  display: flex;
  flex-direction: column;
  width: 100%;
  padding: 0 55px;
}

form {
  display: flex;
  flex-direction: column;
  margin-top: 20px;

  label {
    font-size: 12px;
    font-weight: bold;
    color: #ff9300;
  }

  .form-input {
    margin: 5px 0 10px;
    border:1px solid #ff9300;
    border-top: none;
    border-left: none;
    border-right: none;
    font-size: 14px;
  }

  .form-submit {
    margin: 20px 0;
    background: #00bfd6;
    border-radius: 5px;
    color: #fff;
    text-transform: uppercase;
    font-weight: bold;
    font-size: 14px;
    height: 40px;
    width: 120px;
    align-self: flex-end;
  }
}
</style>
