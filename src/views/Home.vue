<template>
  <q-page class="flex flex-center">
    <img alt="Vue logo" src="../assets/logo.png" />
    <div>{{ version }}</div>
  </q-page>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'

@Options({})
export default class Home extends Vue {
  get version(): string {
    return process.env.VUE_APP_VERSION
  }
}
</script>
