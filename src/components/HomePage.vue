<template>
  <div class="hello">
    <div class="chart-wrapper">
      <Bar id="my-chart-id" :options="chartOptions" :data="chartData" />
    </div>
  </div>
</template>
<script>
import { Bar } from 'vue-chartjs'
import { Chart as ChartJS, Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale } from 'chart.js'

ChartJS.register(Title, Tooltip, Legend, BarElement, CategoryScale, LinearScale)

export default {
  name: 'HomePage',
  data() {
    return {
      chartData: {
        labels: ['January', 'February', 'March'],
        datasets: [{ data: [40, 20, 12] }]
      },
      chartOptions: {
        responsive: true
      }
    }
  },
  props: {

  },
  components: {
    Bar
  },
  methods: {
  },
  computed: {
    myStyles() {
      return {
        height: `${150}px`,
        position: 'relative'
      }
    }

  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
.chart-wrapper{
  border: 1px solid black;
  height: 30vh;
  width: 60vh;
  justify-content: center;
    align-items: center;
    display: inline-flex;
    margin-top:10vh
}
</style>
