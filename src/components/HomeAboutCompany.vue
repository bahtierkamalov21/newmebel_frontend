<template lang="pug">
section(id="about")
  v-row(class="over-content")
    v-col
      v-sheet(class="left" width="680" color="#c5c9c7")
        div
          h2(class="text-center font-weight-regular mb-6") НАША КОМПАНИЯ И УСЛУГИ
          v-sheet(class="left-text ma-auto" max-width="576" color="transparent")
            | Мы осуществляем широкий спектр услуг в сфере реставрации мебели:
            | замена обивки, замена наполнителя, полная и частичная перетяжка, реставрация
            | мягкой мебели, перетяжка кожей.
            | На сайте Вы можете произвести примерный расчёт реставрационных работ.
            | Для того, чтобы получить консультацию и более точный расчёт, свяжитесь
            | с нами по телефону или закажите обратный звонок.
    v-col
      v-sheet(class="right" width="974" height="642")
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeAboutCompany",
});
</script>

<style scoped lang="scss">
#about {
  padding: 160px 0;
  overflow: hidden;
}

.over-content {
  & > * {
    position: relative;
    width: 50%;

    &:last-child {
      position: relative;
      right: 36px;
    }
  }
}

.left {
  position: absolute;
  padding: 80px 24px;
  z-index: 2;
  top: 76px;
  right: -70px;

  &-text {
    font-size: 26px;
  }
}

.right {
  background-image: url("../assets/backgrounds/home-about-company-background.png");
  background-repeat: no-repeat;
  background-size: cover;
}

h2 {
  font-size: 44px;
}
</style>
