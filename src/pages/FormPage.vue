<template>
  <q-page>
    <InputComponent />
  </q-page>
</template>
<script lang="ts">
import InputComponent from 'src/components/InputComponent.vue'
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'FormPage',
  components: { InputComponent }
})
</script>
<style></style>
