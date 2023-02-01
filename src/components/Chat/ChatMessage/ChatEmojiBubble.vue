<script setup>
// A chat bubble container

import useIcons from "../../../compositionFunctions/useIcons";

const icons = useIcons();

const props = defineProps({
  emojiSelect : String,
  direction: {
    type: String,
    default: "right",
  },
});

// Import CSS variables from a 'hook'
</script>

<template>
  <img :src="icons[emojiSelect]" :alt="emoji" :style="cssVars" />
</template>

<style scoped>
img {
  width: 90px;
  height: 90px;
}
</style>