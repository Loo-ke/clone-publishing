<template>
  <svg
    xmlns="http://www.w3.org/2000/svg"
    xmlns:xlink="http://www.w3.org/1999/xlink"
    width="14"
    height="14"
    viewBox="0 0 14 14"
    fill="none"
  >
    <rect width="14" height="14" fill="url(#pattern0_14_315)" />
    <defs>
      <pattern
        id="pattern0_14_315"
        patternContentUnits="objectBoundingBox"
        width="1"
        height="1"
      >
        <use xlink:href="#image0_14_315" transform="scale(0.0138889)" />
      </pattern>
      <image
        id="image0_14_315"
        width="72"
        height="72"
        xlink:href="data:image/png;base64,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"
      />
    </defs>
  </svg>
</template>

<script>
export default defineComponent({
  name: 'IconLogoIt',
})
</script>
