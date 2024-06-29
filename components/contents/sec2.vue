<template>
  <div class="border-t flex justify-between items-start p-6 gap-6">
    <div class="flex flex-col gap-4">
      <div class="text-[#757575] text-sm font-medium">{{ category }}</div>
      <div class="space-y-2">
        <div class="text-lg font-medium">
          {{ title }}
        </div>
        <div class="space-x-2 text-[#424242] text-sm font-medium">
          <span>{{ min }}</span>
          <span>|</span>
          <span>{{ day }}</span>
        </div>
      </div>
      <UserProfile :userImg="props.userImg" :userName="props.userName" />
    </div>
    <div class="bg-gray-200 min-w-24 min-h-24 rounded-lg">{{ img }}</div>
  </div>
</template>
<script setup lang="ts">
const props = defineProps({
  category: String,
  title: String,
  day: String,
  min: String,
  img: String,
  userImg: String,
  userName: String,
})
</script>
