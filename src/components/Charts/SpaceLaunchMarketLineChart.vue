<template>
  <apex-charts
    type="line"
    :options="options"
    :series="series"
  />
</template>

<script>
import spaceLaunchMarket from '../../data/space_launch_market.json'

export default {
  name: 'SpaceLaunchMarketLineChart',

  data() {
    return {
      options: {
        chart: { type: 'line', stacked: false, },
        title: { text: 'Space Launch Market Competition' },
        xaxis: {
          title: { text: 'Year' },
          categories: [
            2010, 2011, 2012, 2013, 2014, 2015, 2016, 2017, 2018, 2019, 2020
          ]
        },
        yaxis: {
          title: { text: 'Number of Launches' },
        }
      },
      series: spaceLaunchMarket,
    }
  },
}
</script>

<style>

</style>
