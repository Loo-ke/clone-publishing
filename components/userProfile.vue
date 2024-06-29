<template>
  <div class="text-xs text-[#9E9E9E] space-x-2">
    <span>{{ userImg == '' ? 'img' : userImg }}</span>
    <span>{{ userName }}</span>
  </div>
</template>
<script setup>
const props = defineProps({
  userImg: String,
  userName: String,
})
</script>
