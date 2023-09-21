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

    <q-drawer v-model="drawer" show-if-above :width="270" :breakpoint="400" elevated class="bg-grey-10 text-white">
      <q-scroll-area style="height: calc(100% - 150px); margin-top: 150px;">
        <q-list class="q-mt-lg">
          <q-item clickable v-ripple href="https://github.com/muriloCoelho1212" target="_blank">
            <q-item-section avatar>
              <q-icon name="fa-brands fa-github" />
            </q-item-section>
            <q-item-section class="text-subtitle2">
              GitHub
            </q-item-section>
          </q-item>
          <q-item clickable v-ripple href="https://www.linkedin.com/in/murilo-coelho-359a23271" target="_blank">
            <q-item-section avatar>
              <q-icon name="fa-brands fa-linkedin" />
            </q-item-section>
            <q-item-section class="text-subtitle2">
              LinkedIn
            </q-item-section>
          </q-item>
        </q-list>
      </q-scroll-area>

      <q-img class="absolute-top bg-grey-9 border" style="height: 157px;">
        <div class="absolute-bottom bg-transparent">
          <q-avatar size="56px" class="q-my-lg">
            <img src="https://cdn.quasar.dev/img/boy-avatar.png">
          </q-avatar>
          <div class="text-weight-bold">Murilo Coelho</div>
        </div>
      </q-img>
    </q-drawer>
  </div>
</template>
<script>
import { defineComponent, ref } from 'vue'
import BreadCrumbsComponent from './BreadCrumbsComponent.vue'

export default defineComponent({
  name: 'HeaderComponent',
  // eslint-disable-next-line space-before-function-paren
  setup() {
    const drawer = ref(false)
    return {
      drawer
    }
  },
  // eslint-disable-next-line space-before-function-paren
  components: { BreadCrumbsComponent }
})
</script>
