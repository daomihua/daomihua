<template>
  <div id="app">
    
    <video autoplay muted loop class="big-bg">
      <source src="./assets/gold.mp4">
    </video>
    <div class="bg"></div>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>
<style>
  body,html{
    width: 100%;
    height: 100%;
    margin:0;
    padding:0;
    box-sizing:border-box;
    background:#f0f0f0f0;
  }
    
  #app {
    position: relative;
    width: 100%;
    height: 100%;
  }
  .big-bg{
    margin: 0; padding: 0;
    position: fixed;
    z-index: -999;
    width: auto;
    height: auto;
    min-width: 100%;
    min-height: 100%;
    top: 0;
    left: 0;
  }
  .bg{
    position: fixed;
    z-index: -998;
    width: 100%;
    height: 100%;
    right: 0;
    bottom: 0;
    background-color: rgba(255, 255, 255, 0.3);
  }
    
</style>




