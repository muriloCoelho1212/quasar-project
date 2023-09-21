<template>
  <q-toolbar class="bg-blue-grey-5 border">
    <q-breadcrumbs active-color="white" class="text-h6 q-pa-md">
      <q-breadcrumbs-el label="Home" icon="home" to="/" />
      <q-breadcrumbs-el label="Cadastro" icon="save_as" to="/register" />
      <q-breadcrumbs-el label="Toolbar" icon="build" />
    </q-breadcrumbs>
  </q-toolbar>
</template>
<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'BreadcrumbsComponent'
})
</script>
<style scoped>
.border {
  border-bottom: 2px solid #9E9E9E;
}
</style>
