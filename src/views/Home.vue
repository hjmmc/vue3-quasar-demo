<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
  </div>
  <div>{{ version }}</div>
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
