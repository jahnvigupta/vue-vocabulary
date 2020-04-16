<template>
<div class="?has-text-white">
<svg
xmlns="http://www.w3.org/2000/svg"
preserveAspectRatio="xMidyMid meet"
viewBox="0 0 304 73">
<use></use>
</svg></div>
</template>

<script>
  export default {
    name: 'Logo',
    props: {
      height: {
        type: Number
      },
      viewBoxX: {
        type: Number
      },
      viewBoxY: {
        type: Number
      },
      fileName: {
        type: String
      },
      id: {
        type: String
      }
    }
  }
</script>
