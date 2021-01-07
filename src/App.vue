<template>
  <div id="app">
    <div id="nav">
      <top-header></top-header>
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    </div>
    <router-view />
  </div>
</template>
<script>
import TopHeader from "@/components/TopHeader.vue";
export default {
  components: {
    "top-header" : TopHeader
    }

}


</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #fff;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}

.shrink {
  transform: scale(0.9);
  padding: 0% 10% 10% 10%;
  box-shadow: 10px solid black;
  }

  .jumbo {
    background-color: #FFA327;
    margin: 0px 100px 0px 100px;
    }

    .bg-info {
    background-color: #FFA327!important;
}
</style>
