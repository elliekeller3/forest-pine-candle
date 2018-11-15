
<template>
  <div>
    <table class="table" v-on:click="penisPenis">
      <thead>
        <tr>
          <th v-for="element in headers"
              :key="element"
              class="border-bottom">
            {{element}}
          </th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td class="border" v-for="cock in cells" :key="cock">
           {{cock}}
          </td>
          
        </tr>
        <tr>
          <td class="border" v-for="cock in cells" :key="cock">
           {{cock}}
          </td>
          
        </tr>
      </tbody>
    </table>
    <span>{{confirmed? 'You confirmed' : 'You canceled'}}</span>
  </div>
  
</template>

<script>
/* eslint-disable */
export default {
  name: 'table',
  props: {
    headers: Array,
    cells: Array
  },
  methods: {
    penisPenis() {
      if(confirm('hello it\'s me, penisPenis')) {
        this.confirmed = true
      } else {
        this.confirmed = false
      }

    }
  },
  data() {
    return {
      confirmed: null
    }
  }
}
</script>

<style scoped>

.table {
  height: 200px;
  width: 400px;
  box-shadow: 0 0 2px 0 rgba(0,0,0,.14), 0 2px 2px 0 rgba(0,0,0,.12), 0 1px 3px 0 rgba(0,0,0,.2);
  margin: 16px;
  padding: 26px;
  border-collapse: collapse
}

.border-bottom {
  border-bottom: 1px solid gray;
}

.border {
  border: 1px solid gainsboro; 
}

</style>
