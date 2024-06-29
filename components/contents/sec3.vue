<template>
  <div class="p-6 space-y-6 bg-[#FAFAFA]">
    <div class="flex flex-col gap-4 w-full">
      <div class="min-h-24 min-w-28 bg-gray-200">{{ icon }}</div>
      <div v-html="title" class="text-lg font-normal leading-6"></div>
    </div>
    <button
      class="w-full border bg-[#6C15EF] text-base font-medium text-white p-4 rounded-lg cursor-pointer"
    >
      {{ btnTitle }}
    </button>
  </div>
</template>
<script setup>
const props = defineProps({
  title: String,
  icon: String,
  btnTitle: String,
  address: String,
})
</script>
