<template>
  <div>
    <Table v-bind:headers="['Penis', 'Pussy', 'Bum']"/>
    <Table />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import Table from '@/components/Table.vue'

export default {
  name: 'home',
  components: {
    HelloWorld,
    Table
  }
}
</script>
