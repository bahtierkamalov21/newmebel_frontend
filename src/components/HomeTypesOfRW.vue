<template lang="pug">
section(id="services")
  v-container
    v-row(class="top")
      v-col(class="text-center")
        h2 ВИДЫ РЕСТАВРАЦИОННЫХ РАБОТ
        p(class="subtitle") ИНДИВИДУАЛЬНЫЙ ПОДХОД К КАЖДОМУ КЛИЕНТУ!
    v-row
      v-col
        v-carousel(show-arrows="hover" hide-delimiters)
          v-carousel-item
            v-row(style="height: 100%;" align="center" justify="center")
              v-col
                home-types-of-r-w-product-card
              v-col
                home-types-of-r-w-product-card
              v-col
                home-types-of-r-w-product-card
              v-col
                home-types-of-r-w-product-card
</template>

<script>
import { defineComponent } from "vue";

// Components
import HomeTypesOfRWProductCard from "@/components/HomeTypesOfRWProductCard.vue";

export default defineComponent({
  name: "HomeTypesOfRW",

  components: { HomeTypesOfRWProductCard },
});
</script>

<style scoped lang="scss">
#services {
  padding: 108px 0;
}

.top {
  margin-bottom: 120px;
}

h2 {
  font-size: 50px;
}

.subtitle {
  font-size: 30px;
}
</style>
