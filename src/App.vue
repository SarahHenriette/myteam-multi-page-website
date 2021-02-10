<template>
  <div id="app">
    <Navbar/>
    <router-view/>
  </div>
</template>

<script>
import Navbar from './components/Nav'

export default {
  components: { Navbar}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Livvic:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,900&display=swap');
@import './public/sass/colors.scss';
body {
  margin: 0;
}
#app {
  font-family: 'Livvic', sans-serif;

  .btn {
    width: 153px;
    height: 48px;
    border-radius: 24px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .normal-state-light {
    border: 2px solid #FFFFFF;
    box-sizing: border-box;
  }
  p {
    margin: 0;
  }
}

</style>
