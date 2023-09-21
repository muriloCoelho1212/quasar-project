<template>
  <div class="q-pa-md">
    <q-input v-model="text" label="Título" class=" q-pa-sm" rounded standout />
    <q-input v-model="text" label="Descrição" class=" q-pa-sm" rounded standout />
  </div>
</template>
<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
  name: 'InputComponent',
  // eslint-disable-next-line space-before-function-paren
  setup() {
    return {
      text: ref('')
    }
  }
})
</script>
<style></style>
