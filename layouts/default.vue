<template>
  <div class="flex flex-col min-h-screen">
    <LayoutsHeader />
    <div class="flex-grow">
      <slot />
    </div>
    <LayoutsFooter />
  </div>
</template>
