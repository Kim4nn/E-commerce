<template>
  <section class="flex justify-center space-x-5 mb-14">
    <CategoryComponent
      backgroundColor="bg-[#F2FCE4]"
      title="Cake & Milk"
      descriptions="14 items"
      image="./src/assets/Burger.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#FFFCEB]"
      title="Peach"
      descriptions="17 items"
      image="./src/assets/Peach.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#ECFFEC]"
      title="Organic Kiwi"
      descriptions="21 items"
      image="./src/assets/Kiwi.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#FEEFEA]"
      title="Red Apple"
      descriptions="68 items"
      image="./src/assets/Apple.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#FFF3EB]"
      title="Snack"
      descriptions="34 items"
      image="./src/assets/Cereal.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#FFF3FF]"
      title="Black plum"
      descriptions="25 items"
      image="./src/assets/Plum.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#F2FCE4]"
      title="Vegetables"
      descriptions="65 items"
      image="./src/assets/Lettuce.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#FFFCEB]"
      title="Headphone"
      descriptions="33 items"
      image="./src/assets/Headset.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#F2FCE4]"
      title="Cake & Milk"
      descriptions="54 items"
      image="./src/assets/Snack.png"
    />
    <CategoryComponent
      backgroundColor="bg-[#FFF3FF]"
      title="Orange"
      descriptions="63 items"
      image="./src/assets/Orange.png"
    />
  </section>
  <section class="flex justify-center space-x-5">
    <PromotionComponent
      backgroundColor="bg-[#F0E8D5]"
      margin="mt-[27px]"
      title="Everyday Fresh & Clean with Our Products"
      image="./src/assets/Onion.png"
      width="w-[220px]"
      height="h-[205px]"
    />
    <PromotionComponent
      backgroundColor="bg-[#F3E8E8]"
      margin="mt-[60px]"
      title="Make your Breakfast Healthy and Easy"
      image="./src/assets/Juice.png"
      width="w-[204px]"
      height="h-[252px]"
    />
    <PromotionComponent
      backgroundColor="bg-[#E7EAF3]"
      buttonColor="bg-[#FDC040]"
      margin="mt-[60px]"
      title="The best Organic Products Online"
      image="./src/assets/Vegetables.png"
      width="w-[234px]"
      height="h-[262px]"
    />
  </section>
</template>

<script>
import CategoryComponent from "./components/CategoryComponent.vue";
import PromotionComponent from "./components/PromotionComponent.vue";

export default {
  components: { CategoryComponent, PromotionComponent },
};
</script>
