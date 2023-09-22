<template>
  <div>
    <q-header>
      <q-toolbar class="bg-grey-9">

        <q-btn flat round dense icon="menu" class="text-h4" @click="drawer = !drawer" />

        <q-toolbar-title class="text-h2 text-center text-weight-regular q-pa-md q-ml-md">
          Quasar Project
        </q-toolbar-title>

      </q-toolbar>
      <bread-crumbs-component />
    </q-header>

    <SidebarComponent :drawer="drawer" />
  </div>
</template>
<script setup lang="ts">
import { ref } from 'vue'
import BreadCrumbsComponent from './BreadCrumbsComponent.vue'
import SidebarComponent from '../SidebarComponent.vue'

const drawer = ref<boolean>(true)
</script>
