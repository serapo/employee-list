<template>
  <div>
  <div class="container">
      <h1>Employee List</h1><br>
      <ul></ul>
  <ul>
    <li>dfkfklfd</li>
    <li>ffdsfdfd</li>
    <li>fgdfgd</li>
  </ul>
  <ul>
    <li>dfkfklfd</li>
    <li>ffdsfdfd</li>
    <li>fgdfgd</li>
  </ul>
  <ul>
    <li>dfkfklfd</li>
    <li>ffdsfdfd</li>
    <li>fgdfgd</li>
  </ul>
  </div>
</div>
</template>

<script>
export default {
  name: 'EmployeList',
 
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container {
  position: relative;
  background-color: black;
  width: 30%;
  height: 90vh;
  display: flex;
  border-radius: 70px;
  align-content: center;
  justify-content: center;
}
div{
  display: flex;
  align-content: center;
  justify-content: center;
}
ul {
  background-color: aqua;
  width: 30%;
  height: 50px;
  display:grid;
}
</style>
