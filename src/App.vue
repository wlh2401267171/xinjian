<template>
  <div id="app">
    <topbar></topbar> 
     <div id="nav">
      <router-link to="/">未签收</router-link> 
      <router-link to="/about">已签收</router-link>
    </div>
    <router-view/>
  </div>
</template> 
<script>
import topbar from "@/components/topbar.vue"
export default{
  components:{
    topbar,
  }
}

</script>
<style lang="less">
html{
font-size: calc(100vw/7.5);
margin: 0;
padding: 0;
body{
  margin: 0;
padding: 0;
  background-color: #f2f2f2;
}
#app {

  margin:0;
  padding: 0;
}
#nav {
  height: 0.6rem;
  a {
    color: black;
    font-size: 0.48rem;
    margin:0rem 1rem;

    &.router-link-exact-active {
      color: red;
    }
  }
}
}
</style>
