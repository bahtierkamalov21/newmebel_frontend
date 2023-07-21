<template lang="pug">
div
  home-header
  home-types-of-r-w
  home-section-info
  home-about-company
  home-contacts
  home-cost-calculation
  home-our-works
</template>

<script>
import { defineComponent } from "vue";

// Components
import HomeHeader from "@/components/HomeHeader.vue";
import HomeTypesOfRW from "@/components/HomeTypesOfRW.vue";
import HomeSectionInfo from "@/components/HomeSectionInfo.vue";
import HomeAboutCompany from "@/components/HomeAboutCompany.vue";
import HomeContacts from "@/components/HomeContacts.vue";
import HomeCostCalculation from "@/components/HomeCostCalculation.vue";
import HomeOurWorks from "@/components/HomeOurWorks.vue";

export default defineComponent({
  name: "HomeView",

  components: {
    HomeHeader,
    HomeTypesOfRW,
    HomeSectionInfo,
    HomeAboutCompany,
    HomeContacts,
    HomeCostCalculation,
    HomeOurWorks,
  },
});
</script>
