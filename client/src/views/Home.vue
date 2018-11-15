<template>
  <div>
    <Table v-bind:headers="['Penis', 'Pussy', 'Bum']" v-bind:cells="['computer', 'cock', 'balls']"/>
    <Table v-bind:headers="['labia', 'light', 'boob']" v-bind:cells="['different', 'word', 'nipple']"/>
  </div>
</template>

<script>
// @ is an alias to /src
/* eslint-disable */
import HelloWorld from '@/components/HelloWorld.vue'
import Table from '@/components/Table.vue'

export default {
  name: 'home',
  components: {
    Table
  }
}
</script>
