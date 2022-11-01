<template>
  <div class="container">
  <employe-list></employe-list>
  </div>
</template>

<script>
import EmployeList from './components/EmployeList.vue'

export default {
  name: 'App',
  components: {
    EmployeList
  }
}
</script>

<style>
body {
  background-color:darkblue ;
}
</style>
