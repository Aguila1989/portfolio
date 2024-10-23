<script>
import Nav from "@/components/header/Nav.vue";

export default {
  name: "Header",
  components: {Nav
  },
  methods: {
    emitPage(item) {
      this.$emit('showRightPage', item);
    },
    handleClick(item) {
      this.$emit("showRightPage", item)
    }
  }
}
</script>

<template>
  <div class="header">
    <div class="h1">
    <div @click="handleClick('about')" class="circle"></div>
  <h1 @click="handleClick('about')">Demeulenaere Kevin - <span>Software Engineering Student</span></h1>
    </div>
  <Nav @showRightPage="emitPage"/>
  </div>
</template>

<style scoped>
.header{
  background-image: url('/src/assets/css/media/view-3d-modern-abstract-sphere-art.jpg');
  background-size: cover;
  background-position: top;
  padding: 1rem 2rem;
  border-radius: 10rem;
  margin: 1rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: sticky;
  top: 1rem;
  left: 0;
  z-index: 100;

}

h1{
  font-size: 1.5rem;
}

.h1{
  display: flex;
  align-items: center;
  cursor: pointer;
}

.circle{

  width: 2rem;
  height: 2rem;
  background-color: lightpink;
  border-radius: 50%;
  margin-right: 10px;
}
</style>