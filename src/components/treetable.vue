<template>
  <table>
    <tbody>
      <tr is="treetablerow" v-for="item in tableData" :item="item"></tr>
    </tbody>
  </table>
</template>

<script>
import treetablerow from './treetablerow.vue'
export default {
  name: "treetable",
  data(){
    return {
      tableData:[
        {text:'1', children:[
          {text:'1.1', children:[]},
          {text:'1.2', children:[]}
        ]},
        {text:'2', children:[
          {text:'2.1', children:[]},
          {text:'2.2', children:[]}
        ]}
      ]
    }
  },
  components:{
    "treetablerow":treetablerow
  }
}
</script>

<style>

</style>


