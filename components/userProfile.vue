<template>
  <div class="text-xs text-[#9E9E9E] flex justify-start gap-2 items-center">
    <IconUser />
    <span>{{ userName }}</span>
  </div>
</template>
<script setup>
const props = defineProps({
  userImg: String,
  userName: String,
})
</script>
