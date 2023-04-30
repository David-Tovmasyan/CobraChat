<!-- Back End -->

<script setup>
import { ref } from 'vue';

let dataRef = ref({message:"No Data"})

const API = "http://localhost:4000/";

async function updateData(){
    let res = await fetch(API);
    let data = await res.json();
    dataRef.value = data ;
}

let inputModel = ref("");

function sendData(){
    fetch(API+"message",inputModel)
}


</script>

<template>
    <!-- getting data from server    -->
    {{ dataRef.message }}
    <button @click="updateData">Fetch Data</button>
    <!-- sending data to server -->
    <input 
        type="text" 
        v-model="inputModel" 
        placeholder="Message"
        name="message"
    >
    <button @click.prevent="sendData">SendData</button>
</template>

<style scoped>

</style>