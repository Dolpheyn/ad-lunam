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
       <q-list>
         <q-item-label
           header
           class="text-black text-bold"
         >
           Navigation
         </q-item-label>

         <EssentialLink
           v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>
    <q-page-container>
      <router-view />
    </q-page-container>

  </q-layout>
</template>

<script>
import EssentialLink from 'components/EssentialLink.vue'

export default {
  components: {
    EssentialLink
  },
  data() {
    return {
      left: false,
      right: false,
      essentialLinks: [
        {
          title: 'Home',
          link: '/'
        },
        {
          title: 'About',
          link: '/about'
        },
      ]
    }
  }
}
</script>
