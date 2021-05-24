<template>
  <q-layout view="hHh LpR fFf">

    <q-header reveal elevated class="bg-white text-black">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="left = !left" />

        <q-toolbar-title>
          <span class="bank-gothic">
            Ad Lunam - To the Moon 🌑
          </span>
        </q-toolbar-title>

      </q-toolbar>
    </q-header>

    <q-drawer show-if-above v-model="left" side="left" overlay bordered>
      <!-- drawer content -->
      <ul>
        <li>Introduction</li>
        <li>History</li>
        <li>Reusable Rockets</li>
        <ul>
          <li>Falcon 1</li>
          <li>Falcon 9</li>
          <li>Falcon Heavy</li>
          <li>Dragon</li>
        </ul>
        <li>Starship</li>
        <li>Starlink</li>
      </ul>
      <ul>
        <li>link</li>
        <li>to</li>
        <li>SpaceX</li>
        <li>website,</li>
        <li>youtube,</li>
        <li>twitter</li>
      </ul>
    </q-drawer>
    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
export default {
  data() {
    return {
      left: false,
      right: false
    }
  }
}
</script>
