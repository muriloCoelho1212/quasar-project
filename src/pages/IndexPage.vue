<template>
  <q-page class="row justify-center items-start">
    <CardComponent v-for="n in 4" :key="n" />
  </q-page>
</template>

<script lang="ts">
import CardComponent from '../components/CardComponent.vue'
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'IndexPage',
  components: { CardComponent }
})
</script>
