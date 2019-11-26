<template>
  <div id="app">
    <ChartBar />
     <div id="app2" align="center">
        <ChartLine />
    </div>   
   
  </div>

 
    
     


</template>

<script>
import ChartBar from './components/ChartBar.vue';
import ChartLine from './components/ChartLine.vue';


export default {
  
  components: {
    ChartBar,
    ChartLine
  }
}
</script>

<style>
#app {
  text-align: center;
}
</style>
