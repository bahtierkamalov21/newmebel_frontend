<template lang="pug">
section(id="contacts")
  v-container
    v-row
      v-col(class="pt-12")
        h2(class="font-weight-regular text-white mb-7") ВЫПОЛНЯЕМ РАБОТУ В
          br
          | КОРОТКИЕ СРОКИ!
        div(class="subtitle text-white") БЕСПЛАТНАЯ ДОСТАВКА ПО МОСКВЕ И
          br
          | СТИЛЬНЫЕ ПОДУШКИ В ПОДАРОК
      v-col
        v-card(class="card ma-auto" max-width="500")
          v-card-title(class="card-title text-center") СВЯЖИТЕСЬ С НАМИ И МЫ
            br
            | ОТВЕТИМ НА ВСЕ ВАШИ ВОПРОСЫ
          v-form(
            class="px-12 mt-10"
            v-model="form"
            @submit.prevent="onSubmit"
          )
            v-text-field(
              v-model="first_name"
              label="Имя"
              type="text"
              variant="solo"
              density="compact"
            )
            v-text-field(
              v-model="phone_number"
              label="Телефон"
              type="tel"
              variant="solo"
              density="compact"
            )
            v-btn(
              :disabled="!form"
              height="86"
              rounded="8"
              color="#16a2eb"
              type="submit"
              block
              class="submit font-weight-regular text-white text-none"
            ) Заказать обратный звонок
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeContacts",

  data: () => ({
    form: false,
    first_name: null,
    phone_number: null,
  }),
  methods: {
    onSubmit() {},
  },
});
</script>

<style scoped lang="scss">
#contacts {
  padding: 126px 0;
  background-image: url("../assets/backgrounds/home-contacts-background.png");
  background-size: cover;
  background-repeat: no-repeat;
}

h2 {
  font-size: 48px;
  line-height: 68px;
}

.subtitle {
  font-size: 28px;
}

.card {
  padding-top: 52px;
  padding-bottom: 80px;
  background-color: rgba(228, 228, 228, 0.75);

  &-title {
    font-size: 26px;
  }
}

.submit {
  font-size: 20px;
}
</style>
