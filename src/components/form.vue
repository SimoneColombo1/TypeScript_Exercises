

<script setup lang="ts">
import { ref } from 'vue'
const name = ref<string>('')
const age = ref<number>(0)


</script>

<template>
<form>
    <label for="name">Name</label>
    <input type="text" id="name" v-model="name" />
    <label for="age">Age</label>    
    <input type="number" id="age" v-model="age" />

    {{ name }}, {{ age }}
</form>


</template>

<style scoped></style>