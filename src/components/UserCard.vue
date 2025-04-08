<script setup lang="ts">
import type {User} from '../Types/User.ts'
const props = defineProps<{
  user: User
}>()

</script>

<template>

  <ul>
    <li>{{ props.user.name }}</li>
    <li>{{ props.user.age }}</li>
    <li v-if="props.user.isAdmin == true">Admin</li>
    <li v-else>Not Admin</li>
  </ul>
</template>

<style scoped></style>
