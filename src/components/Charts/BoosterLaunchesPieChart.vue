<template>
  <apex-charts
    type="pie"
    :options="options"
    :series="series"
  />
</template>

<script>
import boosterLaunches from '../../data/booster_launches.json'
export default {
  name: 'BoosterLaunchesPieChart',

  data() {
    return {
      options: {
        chart: {
          width: 380,
          type: 'pie',
        },
        title: {
          text: 'Block 5 Booster Launches by Landing Status'
        },
        labels: ['Successful Landings', 'Failed Landings'],
        theme: {
          palette: 'palette8'
        },
        responsive: [{
          breakpoint: 2080,
          options: {
            chart: {
              width: 700
            },
          }
        }]
      },
      series: [],
    }
  },

  async created() {
    const launches = boosterLaunches.map(b => b.launches)
    const successfulLandings = boosterLaunches.map(b => b.landing_success)
    const failedLandings = launches.map(
      (launch, i) => launch - successfulLandings[i]
    )

    const total = arr => arr.reduce((acc, val) => acc + val, 0)

    this.series = [
      total(successfulLandings),
      total(failedLandings),
    ]
  }
}
</script>

<style>

</style>
