<script setup >

// Option API //
// export default {
//     data() {
//         return {
//             count: 0
//         }
//     },
//     methods: {
//         increment() {
//             this.count
//         },
//         decrement() {
//             this.count
//         },
//         resetCount() {
//             this.count = 0;
//         }
//     }
// }

// Composition API // scrie <script setup> inainte de a folosi
import { ref } from 'vue';
let count = ref(0);
function resetCount() {
    count.value = 0;
}
</script>

<template>
<div class="myApp">
    <div>
        <h1 class="myTitle">Adauga sau scade valoarea</h1>
        <p class="subTitle">Primul meu component in VueJS</p>
        <h1 class="myValue">{{ count }}</h1>
    </div>
    <div class="btnContainer">
        <button class="btnStyle" @click="count--">Scade</button>
        <button class="btnStyle" @click="resetCount">RESET</button>
        <button class="btnStyle" @click="count++ , !show">Adauga</button>
    </div>
</div>
</template>

<style>
.myApp {
    align-items: center;
    justify-content: center;
    text-align: center;
    background-color: #dedbdb;
    border-bottom: 3px solid #979797;
}
.myTitle {
    font-size: 30px;
    padding: 20px;
}
.mySubTitle {
    font-size: 40px;
}
.myValue {
    font-size: 10rem;
    font-weight: lighter;
    margin-top: 20px;
    margin-bottom: 20px;
    
}
.btnContainer {
    margin-bottom: 20px;
    display: flex;
    justify-content: center;
    gap: 20px;
}
.btnStyle {
    padding: 10px 20px;
    font-size: 1rem;
    color: white;
    background-color: #ff9a03;
    border: 1px #979797;
    border-radius: 8px;
    cursor: pointer;
}
.btnStyle:hover {
    background-color: #e17204;
}
</style>