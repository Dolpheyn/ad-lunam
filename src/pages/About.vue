<template>
  <q-page class="page q-pa-xl q-mx-xl">
    <h1 class="text-h2">About</h1>

    <p>
      We are the students from group CS2595A of Bachelor of Systems
      in Intelligent Systems Engineering from UiTM. This site is one
      of the group assignment deliverables for the subject: Data
      Representation and Reporting Techniques(DSC651).
    </p>

    <p class="q-mb-xl">
      We aim to tell the story of SpaceX, its history, current
      state and plans. Apart from that, we focus on providing
      interactive visualization of SpaceX's past launches and
      missions along with its customers and partners that were
      involved in those missions. Next, we wanted to show the
      characteristics of SpaceX's rockets that have been
      successfully reused through visualizations.
    </p>

    <div style="width: 100%;" class="row justify-center">
      <q-card-section horizontal class="q-mb-md">
        <q-img
          src="../assets/faris.jpg"
          spinner-color="white"
          style="height: 140px; max-width: 150px"
        />

        <div class="q-ma-xl text-h6">
          Muhammad Faris Sufyan Bin Suhaimi (2020953755)
        </div>
      </q-card-section>

      <q-card-section horizontal class="q-mb-md">
        <div class="q-ma-xl text-h6">
          Syamimi Binti Abdul Khalil (2020988399)
        </div>

        <q-img
          src="../assets/mimi.jpg"
          spinner-color="white"
          style="
          height: 140px; max-width: 150px;
          "
        />
      </q-card-section>

      <q-card-section horizontal class="q-mb-md">
        <q-img
          src="../assets/nuqqies.jpg"
          spinner-color="white"
          style="height: 140px; max-width: 150px"
        />

        <div class="q-ma-xl text-h6">
          Khairunuqman Bin Zainal ‘Abidin (2020980287)
        </div>
      </q-card-section>

      <q-card-section horizontal class="q-mb-md">
        <div class="q-ma-xl text-h6">
          Muhammad Arif Bin Ruszaini (2020968445)
        </div>

        <q-img
          src="../assets/areppo.jpg"
          spinner-color="white"
          style="height: 140px; max-width: 150px"
        />
      </q-card-section>
    </div>

    <h1 class="text-h2">Data Sources</h1>

    <p>
      The sources of data we used to create the visualizations:
    </p>

    <q-list bordered separator>
      <q-item
        clickable
        v-ripple
        tag="a"
        target="_blank"
        v-for="dataSource in dataSources"
        :key="dataSource.title"
        :href="dataSource.link"
      >
        <q-item-section>
          <q-item-label>{{dataSource.title}}</q-item-label>

          <q-item-label caption>
            {{dataSource.caption}}
          </q-item-label>
        </q-item-section>
      </q-item>
    </q-list>
  </q-page>
</template>

<script>
const dataSources = [
  {
    title: 'r/SpaceX API',
    caption: '🚀 Open Source REST API for SpaceX launch, rocket, core, capsule, starlink, launchpad, and landing pad data.',
    link: 'https://github.com/r-spacex/SpaceX-API'
  },
  {
    title: 'Wikipedia',
    caption: 'List of Falcon 9 first-stage boosters',
    link: 'https://en.wikipedia.org/wiki/List_of_Falcon_9_first-stage_boosters'
  },
  {
    title: 'Wikipedia',
    caption: 'Space launch market competition',
    link: 'https://en.wikipedia.org/wiki/Space_launch_market_competition'
  },
]
export default {
  name: 'PageIndex',

  data() {
    return {
      dataSources
    }
  }
}
</script>
