<template>
     <p>{{aciklama}}</p>
<div class="emulated-flex-gap" v-for="item of  employe.slice(5,10)  " :key="item.id">
    
    <div>
        <li><img :src="item.image" alt=""></li>
        <li class="name">{{item.name }}</li>
        <li>{{item.email}}</li>
        <li>{{item.age}} years </li>
    </div>
   
    <!-- <img :src="item.image" alt="">
        {{item.name }} <br>{{item.email}} <br>{{item.age}} years -->
</div>
</template>

<script>
import data from '../helper/data'
export default {
    name: "App",

    data() {
        return {
            employe: data,
            number: 5,
            firstDizi: "",
            secondDizi: ""
        };
    },
    props:["aciklama"],
    watch: {
        Next() {
            console.log("jvkkdffd")
            //console.log(this.newStatuId,this.newStatuRadio)

        }
    }
};
</script>

<style scoped>
.name {
    padding: 1rem;
    font-size: 20px;
}

div {
    height: 14vh;

}

img {
    border-radius: 70%;
    width: 90px;
    float: left;
    margin: 1rem;
    margin-left: 3rem;

}

li {
    list-style: none;
    color: black;
}

.emulated-flex-gap>* {
    margin: 15px 0 0 5px;
    background-color: gray;
    width: 100%;
    border-radius: 70px;
    height: 12vh;

}

.emulated-flex-gap {
    display: inline-flex;
    flex-wrap: wrap;
    margin: -10px 0 0 -10px;
    width: calc(100% + 8px);
}
</style>
