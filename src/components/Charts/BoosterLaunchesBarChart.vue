<template>
  <apex-charts
    type="bar"
    :options="options"
    :series="series"
  />
</template>

<script>
import boosterLaunches from '../../data/booster_launches.json'
export default {
  name: 'BoosterLaunchesBarChart',

  data() {
    return {
      options: {
        chart: {
          id: 'booster-launches-bar-chart',
          type: 'bar',
          stacked: true,
        },
        title: {
          text: 'Block 5 Booster Launches'
        },
        xaxis: {
          categories: []
        },
        theme: {
          palette: 'palette8'
        }
      },
      series: [],
    }
  },

  async created() {
    const boosterNames = boosterLaunches.map(b => b.name)
    const launches = boosterLaunches.map(b => b.launches)
    const successfulLaunches = boosterLaunches.map(b => b.landing_success)
    const failedLaunches = launches.map(
      (launch, i) => launch - successfulLaunches[i]
    )
    const totalLaunches = launches.reduce(
      (acc, val) => acc + val,
      0
    )

    this.options.title.text += ` — Total of ${totalLaunches} Launches.`
    this.options.xaxis.categories = boosterNames
    this.series = [
      { name: 'Successful Landings', data: successfulLaunches },
      { name: 'Failed Landings', data: failedLaunches },
    ]
  }
}
</script>

<style>

</style>
