<script setup lang="ts">
import UserCard from './components/UserCard.vue'
import FormUser from './components/form.vue'
import Task from './components/Task.vue'
import type { User } from './Types/User.ts'
const user:User = {
  name: 'gino',
  age: 40,
  isAdmin: true,
}


</script>

<template>
  <UserCard :user="user" />
<FormUser/>
<Task/>

</template>

<style scoped></style>
