<script setup>
import { ref } from 'vue'
const msg = ref('Hello World!')
</script>

<template>
    <div class="myApp">
        <h1 class="myTitle">Scrie si vezi</h1>
        <Child class="subTitle" v-model="msg" />
        <h2 class="subTitle">{{ msg }}</h2>
        
        <span class="subTitle">Scrie ceva</span> <input v-model="msg">
    </div>
</template>

<style >
input {
    padding: 10px;
    margin: 10px 0;
    border: 2px solid #a7a7a7;
    border-radius: 10px;
}
</style>