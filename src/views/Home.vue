<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    {{ v }}
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'

@Options({})
export default class Home extends Vue {
  v = '11'
}
</script>
