<template>
  <div class="flex justify-center space-x-5 mb-14">
    <CategoryComponent
      v-for="category in categories"
      :key="category"
      :background-color="category.color"
      :descriptions="category.productCount"
      :image="category.image"
      :title="category.name"
    />
  </div>
  <div class="flex justify-center space-x-5">
    <PromotionComponent
      v-for="promotion in promotions"
      :key="promotion"
      :background-color="promotion.color"
      :button-color="promotion.buttonColor"
      :image="promotion.image"
      :title="promotion.title"
    />
  </div>
</template>

<script>
import CategoryComponent from "./components/CategoryComponent.vue";
import PromotionComponent from "./components/PromotionComponent.vue";
import axios from "axios";

export default {
  components: { CategoryComponent, PromotionComponent },
  data() {
    return {
      categories: [],
      promotions: [],
    };
  },
  methods: {
    fetchCategories() {
      axios
        .get("http://localhost:3000/api/categories")
        .then((response) => {
          this.categories = response.data;
        })
        .catch((error) => {
          console.log("Error fetching data:", error);
        });
    },
    fetchPromotions() {
      axios
        .get("http://localhost:3000/api/promotions")
        .then((response) => {
          this.promotions = response.data;
        })
        .catch((error) => {
          console.log("Error fetching data:", error);
        });
    },
  },
  mounted() {
    this.fetchCategories();
    this.fetchPromotions();
  },
};
</script>
