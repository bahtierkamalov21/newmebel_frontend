<template lang="pug">
v-footer(class="d-flex flex-column")
  div(class="mb-14")
    v-row
      v-col(class="text-center")
        h2(class="size-text") ОСТАЛИСЬ ВОПРОСЫ?
          br
          | СВЯЖИТЕСЬ С НАМИ!
  div
    v-row(class="cols" justify="center" align="center")
      v-col(class="col" cols="auto")
        a(
          class="size-text d-block text-decoration-none text-black mb-2"
          href="tel:+79680000799"
        ) +7 968 000 07 99
        a(
          class="size-text d-block text-decoration-none text-black"
          href="mailto:info@instagram.ru"
        ) info@instagram.ru
      v-col(class="text-center col col-centering" cols="auto")
        div(class="size-text") Время работы:
          br
          | 08:00 – 22:00
      v-col(class="col" cols="auto")
        a(
          href="#"
          target="_blank"
          class="social-link size-text d-flex align-center text-decoration-none text-black"
          style="gap: 24px;"
        )
          img(src="../assets/icons/telegram-icon.svg" alt="telegram-icon")
          | Telegram
        a(
          href="#"
          target="_blank"
          class="social-link size-text d-flex align-center text-decoration-none text-black"
          style="gap: 24px;"
        )
          img(src="../assets/icons/instagram-icon.svg" alt="telegram-icon")
          | Instagram
  div(class="mt-6 mb-4") Powered by NEW Mebel
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeFooter",
});
</script>

<style scoped lang="scss">
.size-text {
  font-size: 34px;
}

.col {
  padding: 32px 100px;

  &-centering {
    border-top: 0;
    border-bottom: 0;
    border-right: 2px;
    border-left: 2px;
    border-style: solid;
    border-color: black;
  }
}

.cols {
  & > *:first-child {
    padding-left: 20px;
  }

  & > *:last-child {
    padding-right: 20px;
  }
}
</style>
