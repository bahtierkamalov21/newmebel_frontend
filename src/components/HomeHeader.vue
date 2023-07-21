<template lang="pug">
header(class="py-10")
  v-container
    v-row
      v-col
        h1(class="text-white mb-7") Хотите восстановить любимый
          br
          | диван или кресло?
        h2(class="text-white") Напишите нам и мы вдохнем в неё новую жизнь!
        v-btn(
          size="x-large"
          class="button text-none text-white"
          width="548"
          height="86"
          color="#16a2eb"
        ) Связаться с нами
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeHeader",
});
</script>

<style scoped lang="scss">
header {
  background-image: url("../assets/backgrounds/home-header-background.png");
  background-repeat: no-repeat;
  background-size: cover;
}

h1 {
  font-size: 36px;
  line-height: 36px;
}

.button {
  font-size: 32px;
  margin-top: 100px;
  margin-bottom: 226px;
}
</style>
