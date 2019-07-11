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
