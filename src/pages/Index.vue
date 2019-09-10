import { Platform } from 'quasar'

<template>
  <q-page class="flex flex-center">
    <q-badge color="primary">2019 {{ myInfiniteVariable }}-09</q-badge>
    {{ $q.platform }}
  </q-page>
</template>

<style>
</style>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      myInfiniteVariable: true
    }
  }
}
</script>
