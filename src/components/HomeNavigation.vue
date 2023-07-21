<template lang="pug">
v-app-bar(elevation="0")
  v-container(class="navigation-container")
    v-row
      v-app-bar-title(class="title")
        router-link(class="text-decoration-none text-black" to="/") NEW Mebel
      v-spacer
      ul(class="navigation-ul d-flex align-center flex-wrap")
        li(v-for="(item, index) in navigation_list" :key="index")
          a(
            :href="item.href"
            :class="{ active: active_link === index }"
            @click="change_active_link(index)"
            class="text-decoration-none font-weight-medium text-black"
          ) {{ item.name }}
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "HomeNavigation",

  data: () => ({
    active_link: null,
    navigation_list: [
      {
        name: "о компании",
        href: "#about",
      },
      {
        name: "услуги",
        href: "#services",
      },
      {
        name: "материалы",
        href: "#materials",
      },
      {
        name: "расчет стомости",
        href: "#calculation",
      },
      {
        name: "наши работы",
        href: "#our_works",
      },
      {
        name: "контакты",
        href: "#contacts",
      },
    ],
  }),
  methods: {
    change_active_link(index) {
      this.active_link = index;
    },
  },
  created() {
    for (let i = 0; i < this.navigation_list.length; i++) {
      if (this.navigation_list[i].href === location.hash) {
        this.change_active_link(i);
        break;
      }
    }
  },
});
</script>

<style scoped lang="scss">
.title {
  font-family: "Merienda", cursive;
  font-size: 30px;
}

.navigation-ul {
  gap: 44px;
  list-style: none;
  padding-right: 66px;

  & > li > a {
    position: relative;

    &:hover {
      &:before {
        transition: 0.5s linear width;
        width: 100%;
      }
    }

    &:before {
      transition: 0.5s linear width;
      content: "";
      width: 0;
      height: 2px;
      background-color: #16a2eb;
      position: absolute;
      right: 0;
      bottom: -10px;
    }
  }
}

.active:before {
  width: 100% !important;
}

@media screen and (min-width: 1512px) {
  .navigation {
    &-container {
      max-width: 1640px !important;
    }

    &-ul {
      padding-right: 32px;
    }
  }
}
</style>
