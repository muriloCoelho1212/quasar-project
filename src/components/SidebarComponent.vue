<template>
  <q-drawer v-model="myDrawer" show-if-above :width="270" :breakpoint="400" elevated class="bg-grey-10 text-white">
    <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px;">
      <q-list class="q-mt-lg">
        <q-item clickable v-ripple href="https://github.com/muriloCoelho1212" target="_blank" class="q-pa-lg">
          <q-item-section avatar>
            <q-icon name="fa-brands fa-github" />
          </q-item-section>
          <q-item-section class="text-subtitle2">
            GitHub
          </q-item-section>
        </q-item>
        <q-item clickable v-ripple href="https://www.linkedin.com/in/murilo-coelho-359a23271" target="_blank"
          class="q-pa-lg">
          <q-item-section avatar>
            <q-icon name="fa-brands fa-linkedin" />
          </q-item-section>
          <q-item-section class="text-subtitle2">
            LinkedIn
          </q-item-section>
        </q-item>
      </q-list>
    </q-scroll-area>

    <div class="absolute-top row bg-transparent items-center justify-center" style="height: 157px;">
      <div class="text-weight-bold text-h6">Murilo Coelho</div>
    </div>
  </q-drawer>
</template>
<script setup lang="ts">
import { computed } from 'vue'

const props = defineProps<{ drawer: boolean }>()

const myDrawer = computed(() => {
  return props.drawer
})

</script>
<style></style>
