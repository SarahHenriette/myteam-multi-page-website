<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link> 
      <router-link to="/contact">Contact us</router-link>
    </div> -->
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



  // -webkit-font-smoothing: antialiased;
  // -moz-osx-font-smoothing: grayscale;
  // text-align: center;
  // color: #2c3e50;
}

// #nav {
//   padding: 30px;

//   a {
//     font-weight: bold;
//     color: #2c3e50;

//     &.router-link-exact-active {
//       color: #42b983;
//     }
//   }
// }
</style>
