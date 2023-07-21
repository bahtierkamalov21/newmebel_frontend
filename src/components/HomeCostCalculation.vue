<template lang="pug">
section(id="calculation")
  v-container
    v-row
      v-col(class="text-center")
        h2(class="font-weight-regular mb-10") РАСCЧИТАЙТЕ СТОИМОСТЬ РАБОТ С
          br
          | ПОМОЩЬЮ НАШЕГО КАЛЬКУЛЯТОРА
        v-btn(
          color="#16a2eb"
          class="button font-weight-regular text-white"
          height="86"
          width="470"
        ) РАССЧИТАТЬ
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeCostCalculation",
});
</script>

<style scoped lang="scss">
#calculation {
  padding: 100px 0;
}

h2 {
  font-size: 40px;
}

.button {
  font-size: 40px;
  border-radius: 76px;
}
</style>
