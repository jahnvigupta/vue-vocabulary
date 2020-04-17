<template>
<div :class="textColor">
<svg style="height: 73px;"
xmlns="http://www.w3.org/2000/svg"
preserveAspectRatio="xMidyMid meet"
:viewBox=viewBox>
<use :href=fileAddress></use>
</svg></div>
</template>

<script>
  export default {
    name: 'Logo',
    props: {
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
      },
      textColor: {
        type: String
      }
    },
    computed: {
      fileAddress () {
        return 'logos/' + this.fileName + '.svg#' + this.id
      },
      viewBox () {
        return '0 0 ' + this.viewBoxX + this.viewBoxY
      }
    }
  }
</script>
