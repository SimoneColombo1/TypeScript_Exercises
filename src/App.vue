<script setup lang="ts">
import UserCard from './components/UserCard.vue'
import type { User } from './Types/User.ts'
const user:User = {
  name: 'gino',
  age: 40,
  isAdmin: true,
}


</script>

<template>
  <UserCard :user="user" />
</template>

<style scoped></style>
