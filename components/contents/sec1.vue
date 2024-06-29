<template>
  <div class="p-6 space-y-6 font-medium">
    <div class="bg-gray-300 h-44 rounded-xl flex justify-center items-center">
      <span>image</span>
      <div></div>
    </div>
    <div class="flex flex-col">
      <div class="pb-2 text-[#757575]">{{ data.category }}</div>
      <div>
        <span class="text-lg">{{ data.title }}</span>
        <div class="text-xs">
          <span>icon {{ data.min }}</span>
          <span>{{ data.day }}</span>
        </div>
      </div>
      <div class="py-3 text-xs text-[#757575]">
        {{ data.desc }}
      </div>
      <UserProfile :userName="data.userName" :userImg="data.userImg" />
    </div>
  </div>
</template>
<script setup>
const props = defineProps({
  data: Object,
})
</script>
