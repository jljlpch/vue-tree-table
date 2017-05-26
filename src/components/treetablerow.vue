<template>
  <div>
    <tr>
      <td>
        {{item.text}}
      </td>
    </tr>
    <tr is="treetablerow" v-for="subItem in item.children" :item="subItem"></tr>
  </div>
</template>

<script>
export default {
  props:["item"],
  name: "treetablerow"
}
</script>

<style>

</style>


