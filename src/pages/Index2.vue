import { Platform } from 'quasar'
import { uid } from 'quasar'

<template>
  <q-page class="flex flex-center">
    {{ $q.platform }} {{ $q.uuid }}
    <q-btn color="purple" to="/map">
      <q-icon left size="3em" name="map" />
      <div>Try this!</div>
    </q-btn>
  </q-page>
</template>

<style>
</style>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      myInfiniteVariable: true,
      uuid: 'hello'
    }
  }
}
</script>
