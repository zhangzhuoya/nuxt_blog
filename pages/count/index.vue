<template>

    <div>
        <h1>
            <button @click="count1++;count2++">+</button>
           count1: {{ 
            count1
             }}
            <button @click="ens">-</button>
        </h1>
        <h2>
           <A></A>
        </h2>
        <h2>
            <B></B>
         </h2>
    </div>
</template>

<script setup lang="ts">
import {useState} from 'nuxt/app'

let count1 = useState("count1",()=> Math.round(Math.random()* 1000))
let count2 = useCounter();
// let countRef = ref(Math.round(Math.random()* 1000))
function add() {
    console.log(124);
    
    // countRef++;
}
function ens() {
    // count--;
    // countRef--;
}
</script>