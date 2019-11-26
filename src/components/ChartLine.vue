<template>
  <div class="app2" style="width:600px; height: 600px">
    <h2>Dezembro</h2>
     <chartjs-line v-bind:labels="labels"  v-bind:option="option"> 

     </chartjs-line>
  </div>
</template>

<script>
export default {
 data(){
   return{
    // labels: ['Muito Feliz', 'Feliz', 'Razoável', 'Triste', 'Muito triste'],
          
     datasets: [
       { label: 'Feliz',
         data: [10, 20, 30, 40, 50],
         backgroundColor:["Red","Yellow", "Blue", "Green", "Purple"]
      },
       { label: 'Triste',
         data: [10, 20, 30, 40, 50],
         backgroundColor:["Red","Yellow", "Blue", "Green", "Purple"]
      }
      ],

      option: {
        title: {
          display: true,
          position: "bottom",
          text: "Moods"
        },
         scales: {
          xAxes: [{
          type: 'category',
          labels: ['Janeiro', 'Fevereiro', 'Março', 'Abril', 'Maio'],
        }],  
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
