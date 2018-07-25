<template>
  <div>
    <headerNav></headerNav>
      <app-server-status v-for="server in 3" :key="server.id"></app-server-status>
  </div>
</template>

<script>
import Headernya from './components/shared/Header.vue'
import Servernya from './components/server/ServerStatus.vue'

export default {
    components: {
      headerNav : Headernya,
      'app-server-status' : Servernya
    }
}
</script>

<style>
</style>
