<template>
<div class="app">
  <h1>hello world</h1>
  <person/>
</div>
</template>

<script lang="ts">
import Person from './components/Person.vue'
export default{
  name:'App',
  components:{Person}

}
</script>

<style>
.app{
  background-color: yellow;
}
</style>