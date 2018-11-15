<template>
  <div>
    <table>
      <thead>
        <tr>
          <th>
            Header 1
          </th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>
            Body 1
          </td>
          <td>
            Body 2
          </td>
        </tr>
      </tbody>
    </table>
  </div>
  
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    headers: Array
  }
}
</script>

<style scoped>
</style>
