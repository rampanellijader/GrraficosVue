<template>
  <div class="app" style="width:600px; height: 600px">
    <h2>Chart Bar</h2>
     <chartjs-bar v-bind:labels="labels" v-bind:datasets="datasets" v-bind:option="option"> 

     </chartjs-bar>
  </div>
</template>

<script>
export default {
 data(){
   return{
     labels: ['Muito Feliz', 'Feliz', 'Razoável', 'Triste', 'Muito triste'],
          
     datasets: [
       {
         data: [10, 20, 30, 40, 50],
         backgroundColor:["Red","Yellow", "Blue", "Green", "Purple"]
      }
      ],

      option: {
        title: {
          display: true,
          position: "bottom",
          text: "Moods",
          responsive: true
        },
         scales: {
         yAxes: [{
         ticks: {
         beginAtZero: true
        }
      }]
    }
      }
   }
  }

}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
