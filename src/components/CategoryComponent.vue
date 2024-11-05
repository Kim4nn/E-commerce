<template>
  <div
    :class="`${backgroundColor} justify-center text-center w-28 h-44 border-none rounded-[10px]`"
  >
    <img :src="image" width="120" height="120" />
    <p class="font-semibold text-base">{{ title }}</p>
    <p class="text-xs text-gray-400 font-medium">{{ descriptions }}</p>
  </div>
</template>

<script>
export default {
  props: {
    backgroundColor: String,
    title: String,
    descriptions: String,
    image: {
      type: String,
      Required: true,
    },
  },
};
</script>
