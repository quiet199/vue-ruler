<template>
    <div id="nav">
        <router-link to="/">Home</router-link> | 
        <router-link to="/csRuler">csRuler</router-link> 
    </div>
</template>

<script>

    export default{
        name: "Home",
        data() {
            return {
            }
        },
    }
</script>

<style lang="less" scoped>
#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>