<script setup lang="ts">
import { ref } from 'vue'
import type { Task } from '../Types/Task.ts'
const tasks = ref<Task[]>([{
id:1,
title:'task 1',
done : false

},
{
id:2,
title:'task 2',
done : false

},
{id:3,
title:'task 3',
done : true
}
])

</script>

<template>

<ul>
 
    <li v-for ="task in tasks" :key="task.id">
        {{ task.title }}
        <span v-if="task.done== true">V</span>
        <span v-else>X</span> </li>
</ul>
</template>

<style scoped></style>
