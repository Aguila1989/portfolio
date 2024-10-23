<script>
import About from "@/components/subPages/about/About.vue";
import Resume from "@/components/subPages/resumePage/Resume.vue";
import Portfolio from "@/components/subPages/portfolio/Portfolio.vue";
import Blog from "@/components/subPages/blog/Blog.vue";
import Contact from "@/components/subPages/contact/Contact.vue";
export default {
  name: "PagesContainer",
  components: {Portfolio, Resume, About, Blog, Contact},
  props: {
    selectedItem: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <template v-if="selectedItem === 'about'">
    <About/>
  </template>
  <template v-if="selectedItem === 'resume'">
    <Resume/>
  </template>
  <template v-if="selectedItem === 'portfolio'">
    <Portfolio/>
  </template>
  <template v-if="selectedItem === 'blog'">
    <Blog/>
  </template>
  <template v-if="selectedItem === 'contact'">
    <Contact/>
  </template>
</template>

<style scoped>

</style>