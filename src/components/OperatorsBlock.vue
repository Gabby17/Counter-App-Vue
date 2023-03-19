<script setup>
import { useOperation } from '../composables/composable';

const {
    increment,
    decrement,
    reset,
    change
} = useOperation()
</script>
<template>
    <div class="grid">
        <button @click="increment">+ Increment</button>
        <button @click="decrement">- Decrement</button>
        <button @click="reset" class="double">Reset</button>
        <input type="number" @change="change" class="double" placeholder="setValue" />
    </div>
</template>

<style scoped>
.grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
}

.double {
    grid-column: 1/-1;
}

input,
button {
    padding: 10px;
    width: 100%;
    border: 3px solid transparent;
    border-radius: 6px;
    color: black;
    transition: 700ms;
    background-color: #ffc700;
}

button:hover {
    border: 3px solid #ffffff;
}

button:active {
    background-color: white;
    color: black;
}
</style>