<template>
<div>
    <div class="container">
        <h1>Employee List</h1>
        <span>Employees {{first }} to {{second}} </span>
        <employesList :firstDizi="firstDizi" :secondDizi="secondDizi" />
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
    },
    data() {
        return {
            first: 1,
            second: 5,
            firstDizi: 1,
            secondDizi: 5
        }
    },
    methods: {
        Next() {
            if (this.first == 16 || this.second == 20) {
                this.first = 1
                this.firstDizi = this.first
                this.second = 5
                this.secondDizi = this.second
              
            } else {
                this.first += 5
                this.firstDizi = this.first
                this.second += 5
                this.secondDizi = this.second
            }
        },
        Prev() {
            if (this.first == 1 && this.second == 5) {
                this.first = 16
                this.firstDizi = this.first
                this.second = 20
                this.secondDizi = this.second
            } else {
                this.first -= 5
                this.firstDizi = this.first
                this.second -= 5
                this.secondDizi = this.second
            }
        }
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
    width: 60%;
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
