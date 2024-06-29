<template>
  <div>
    <contentsSec1 :data="mainData" />
    <contentsSec2
      v-for="data of sec2Data"
      :title="data.title"
      :userName="data.userName"
      :userImg="data.userImg"
      :day="data.day"
      :min="data.min"
      :img="data.img"
    />
    <!-- spacer -->
    <div class="py-2"></div>

    <contentsSec3
      :title="sec3Data[0].title"
      :btnTitle="sec3Data[0].btnTitle"
      :address="sec3Data[0].address"
      :icon="sec3Data[0].icon"
    />
    <div class="pt-8">
      <div class="flex justify-between items-center px-6 py-4">
        <span class="font-medium text-2xl">인기 있는 콘텐츠</span>
        <span class="text-[#6B16EE] text-sm font-medium">더 보기 ></span>
      </div>
    </div>

    <contentsSec1 v-for="data of sec1Data" :data="data" />
    <!-- spacer -->
    <div class="py-10"></div>
    <contentsSec3
      :title="sec3Data[1].title"
      :btnTitle="sec3Data[1].btnTitle"
      :address="sec3Data[1].address"
      :icon="sec3Data[1].icon"
    />
  </div>
</template>
<script setup>
import { mainData, sec2Data, sec3Data, sec1Data } from '~/data/indexData'
</script>
