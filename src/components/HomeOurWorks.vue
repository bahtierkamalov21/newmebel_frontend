<template lang="pug">
section(id="our_works")
  v-container
    v-row
      v-col(class="text-center")
        h2(class="font-weight-regular") НАШИ РАБОТЫ
        h3(class="font-weight-regular") ДАЙТЕ СВОЕЙ МЕБЕЛИ ВТОРОЙ ШАНС!
  v-row(justify="center")
    v-carousel(
      class="carousel"
      hide-delimiters
      show-arrows="hover"
      height="962"
    )
      v-carousel-item
        img(src="../assets/our_works/carousel_image_product.png" alt="chairs")
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeOurWorks",
});
</script>

<style scoped lang="scss">
#our_works {
  padding: 100px 0;
}

h2 {
  font-size: 50px;
}

h3 {
  font-size: 40px;
}

.carousel {
  margin-top: 100px;
  max-width: 1440px;
}
</style>
