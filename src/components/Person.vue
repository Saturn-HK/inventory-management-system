<template>
  <div class="person">
    <h2>student information</h2>
    <li v-for="i in persons" v-bind:key="i.id">student id:{{i.id}}
    <span>
     name:{{i.name}}
    </span>
    </li>
<!--    <h2>student id:{{persons[1].name}}</h2>-->
<!--    <button @click="changename">change name</button>-->
<!--    <button @click="changeage">change age</button>-->
<!--    <button @click="showTel">Check Tel</button>-->
  </div>
</template>

<script lang="ts" setup>


    import {reactive} from 'vue';
    let persons=reactive(
        [
            {id:'20183270029',name:'Huang'},
            {id:'20183270030',name:'Shao'},
            {id:'20183270031',name:'Tong'}])
    function showTel(){


    }
    function changename(){

    }
    function changeage(){

    }
// return {persons, showTel, changename, changeage};


</script>

<style scoped>
.person{
  background-color: skyblue;
  box-shadow: 0 0 10px;
  border-radius: 10px;
  padding:20px;
}
</style>