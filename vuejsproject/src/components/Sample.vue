<template> 
  <div class="hello">
    <h1 :style="cse">HARI</h1>
    <table v-if="isvisible">
    <tr>
    <th>NAME</th>
    <th>AGE</th>
    </tr>
    <tr v-for="Item in person">
    <td>{{Item.name}}</td>
    <td>{{Item.age}}</td>
    </tr>
    </table>
    <h1 v-if="isvisible"> TRUE</h1>
    <h2 v-else> FALSE</h2>
    <button  v-on:click="abc">click here</button>
    <h1> MAHESH</h1>
  </div>
</template>
<script>
export default {
  name: 'Sample',
  data() {
    return{
    person:[{name:"candy",age:20},{name:"sande",age:21},{name:"ande",age:35}],
     isvisible:true,
     cse:{color:'blue',background:'green'
          }
    }
  },
  methods : {
              abc:function() {
                this.isvisible = !this.isvisible              }
            }
         }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1{
   background-color:blue;
   color:red
}
</style>
