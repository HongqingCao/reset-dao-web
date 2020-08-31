<template>
  <div>
   <navBar></navBar>
   <sectionOne></sectionOne>
  </div>
</template>

<script>
import navBar from "@/components/navBar.vue";
import sectionOne from "./components/sectionOne.vue";

export default {
  name: "Home",
  components: {
    navBar,
    sectionOne
  }
};
</script>
