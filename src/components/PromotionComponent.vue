<template>
  <section
    :class="`relative ${backgroundColor} rounded-[10px] w-[420px] h-[300px]`"
  >
    <div class="w-[290px] h-[200px] pt-[65px] pl-[25px]">
      <p class="text-2xl font-semibold">{{ title }}</p>
      <ButtonComponent :title="title" :class="`${buttonColor} mt-[50px]`" />
    </div>
    <div class="absolute bottom-0 right-0">
      <img :src="image" width="220" height="250" />
    </div>
  </section>
</template>

<script>
import ButtonComponent from "./ButtonComponent.vue";

export default {
  components: { ButtonComponent },
  props: {
    backgroundColor: String,
    buttonColor: String,
    image: {
      type: String,
      require: true,
    },
    title: String,
  },
};
</script>
