<template>
  <q-layout view="lHh Lpr lFf">

    <header-component />
    <q-page-container class="bg-grey-4 width">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script lang="ts">
import HeaderComponent from 'src/components/Header/HeaderComponent.vue'
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'MainLayout',
  components: { HeaderComponent }
})
</script>
