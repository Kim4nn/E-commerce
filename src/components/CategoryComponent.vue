<template>
  <section
    :class="`${backgroundColor} justify-center text-center w-28 h-44 border-none rounded-[10px]`"
  >
    <img :src="image" width="120" height="120" />
    <p class="font-semibold text-base">{{ title }}</p>
    <p class="text-xs text-gray-400 font-medium">{{ descriptions }} items</p>
  </section>
</template>

<script>
export default {
  props: {
    backgroundColor: String,
    title: String,
    descriptions: Number,
    image: {
      type: String,
      Required: true,
    },
  },
};
</script>
