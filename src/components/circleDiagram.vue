<template>
  <Doughnut :chart-options="chartOptions" :chart-data="chartData" :width="50" />
</template>

<script>
import { Doughnut } from "vue-chartjs";
import { Chart as ChartJS, Tooltip, Legend, ArcElement } from "chart.js";

ChartJS.register(Tooltip, Legend, ArcElement);
const chartOptions = {
  responsive: true,
  maintainAspectRatio: false,
};
export default {
  name: "BarChart",
  components: { Doughnut },
  data() {
    return {
      chartOptions,
      chartData: {
        labels: ["January", "February", "March"],
        datasets: [
          {
            label: "Data One",
            backgroundColor: ["#f87979", "#000"],
            data: [40, 20, 12],
          },
        ],
      },
    };
  },
};
</script>