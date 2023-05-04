<script lang="ts" setup>
  import { Message, User } from '../types';
  defineProps<{
    messages: Message[]
    users: User[]
    me: User
    usersTyping?: User[]
  }>()

  const isOpen = ref(false)
</script>

<template>
  <div class="fixed bottom right">
    <button>
      <IronChat />
    </button>
  </div>
</template>
