import { Platform } from 'quasar'

<template>
  <q-page class="flex flex-center">
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
