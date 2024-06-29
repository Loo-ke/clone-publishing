<template>
  <header class="pt-3">
    <div
      class="flex gap-2 justify-start items-center text-sm font-medium text-gray-300 px-4"
    >
      <div class="flex gap-1 text-black">
        <div>icon</div>
        <div>요즘 IT</div>
      </div>
      <div>|</div>
      <div class="flex gap-1">
        <div>icon</div>
        <div>위시켓</div>
      </div>
    </div>
    <div class="flex justify-between items-center px-4">
      <div class="py-7">logo</div>
      <ul class="list-none flex justify-end gap-2 items-center">
        <li>
          <div class="text-sm font-medium border rounded-full px-2 py-1">
            작가 지원
          </div>
        </li>
        <li>돋보기</li>
        <li>메뉴</li>
      </ul>
    </div>
    <div class="border-b">
      <nav
        class="flex justify-between items-center gap-7 whitespace-nowrap text-sm font-medium w-full overflow-scroll scrollbar-hide border-b px-4"
      >
        <template v-for="nav of navList">
          <div class="py-3 font-medium text-sm" v-if="!nav.subNav">
            {{ nav.label }}
          </div>
          <template v-for="subNav of nav.subNav">
            <div class="text-xs font-normal">{{ subNav.label }}</div>
          </template>
        </template>
      </nav>
    </div>
  </header>
</template>
<script setup>
const navList = ref([
  {
    key: 'new',
    label: '새로 나온',
  },
  {
    key: 'hit',
    label: '인기',
  },
  {
    key: 'recentWritter',
    label: '요즘 작가들',
  },
  {
    key: 'ask',
    label: '물어봐',
  },
  {
    subNav: [
      {
        key: 'plan',
        label: '기획',
      },
      {
        key: 'design',
        label: '디자인',
      },

      {
        key: 'product',
        label: '프로덕트',
      },
      {
        key: 'outsourcing',
        label: '아웃소싱',
      },
      {
        key: 'freelancing',
        label: '프리랜싱',
      },
      {
        key: 'business',
        label: '비지니스',
      },
      {
        key: 'IT',
        label: 'IT서비스',
      },
    ],
  },
])
</script>
