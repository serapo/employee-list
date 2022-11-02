<template>
<div>
    <div class="container">
        <h1>Employee List</h1>
        <span>Employees 1 to 5 </span>
        <employesList />
        <button @click="Prev" type="button" class="btn btn-primary">Prev</button>
        <button @click="Next" type="button" class="btn btn-primary">Next</button>
    </div>
</div>
</template>

<script>
import EmployesList from './EmployesList.vue'
export default {
    name: 'EmployeList',
    components: {
        EmployesList,

    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style scoped>
button {
    margin: 2rem;
    width: 7rem;
}

.container {
    position: relative;
    background-color: black;
    width: 50%;
    height: 90vh;
    display: flex;
    border-radius: 70px;
    align-content: center;
    justify-content: center;
    display: block;
    padding: 1rem;
    text-align: center;
    
}

h1 {
    background-color: blueviolet;
    height: 5rem;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    border-radius: 70px;
}

div {
    display: flex;
    align-content: center;
    justify-content: center;
}
span {
  margin: 5rem;
  padding: 5rem;
}
</style>
