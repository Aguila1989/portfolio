<script>
import Header from "@/components/header/Header.vue";
import PagesContainer from "@/components/PagesContainer.vue";

export default {
  name: "MainPage",
  components: {PagesContainer, Header},
  data() {
    return {
      selectedItem: "about"
    };
  }
}
</script>

<template class="main-page">
  <Header @showRightPage="selectedItem = $event"/>
  <PagesContainer :selected-item="selectedItem"/>
</template>

<style scoped>

</style>