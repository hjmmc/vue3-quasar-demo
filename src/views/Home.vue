<template>
  <q-page>
    <q-banner class="bg-primary text-white">
      Unfortunately, the credit card did not go through, please try again.
      <template v-slot:action>
        <q-btn flat color="white" label="Dismiss" />
        <q-btn flat color="white" label="Update Credit Card" />
      </template>
    </q-banner>
    <div class="flex flex-center">
      <img alt="Vue logo" src="../assets/logo.png" />
      <div>{{ version }}</div>
    </div>
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
