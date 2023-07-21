<template lang="pug">
v-card(width="222" class="ma-auto" elevation="0" rounded="0")
  img(
    src="../assets/products/product_one.png"
    alt="Кресла и стулья"
    width="222"
    height="242"
  )
  v-card-title(class="card-title px-0 pt-8 pb-10") Кресла и стулья
  v-card-text(class="pa-0 text-black")
    ul(class="d-flex flex-column")
      li Ткань - от 1200 руб.
      li Экокожа - от 1300 руб
      li Натуральная кожа - от 2500 руб
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeTypesOfRWProductCard",
});
</script>

<style scoped lang="scss">
.card-title {
  font-size: 28px;
}

ul {
  list-style: none;
  gap: 12px;

  & > li {
    font-size: 20px;
  }
}
</style>
