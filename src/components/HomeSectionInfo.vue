<template lang="pug">
section(class="info")
  v-container
    v-row
      v-col(align="center")
        v-sheet(class="text-center pt-12 pb-10" width="730")
          h2(class="font-weight-regular") Выполняем работу у Вас на дому
            br
            | или в нашей мастерской!
            br
            | Работаем по Москве и МО
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeSectionInfo",
});
</script>

<style scoped lang="scss">
.info {
  padding: 102px 0;
  background-image: url("../assets/backgrounds/home-info-background.png");
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
