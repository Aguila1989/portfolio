<script>
import Nav from "@/components/header/Nav.vue";

export default {
  name: "Header",
  components: {
    Nav
  },
  methods: {
    emitPage(item) {
      this.$emit('showRightPage', item);
    },
    handleClick(item) {
      this.$emit("showRightPage", item);
    }
  }
};
</script>

<template>
  <header>
    <div class="h1">
      <div @click="handleClick('about')" class="circle"></div>
      <h1 @click="handleClick('about')">Demeulenaere Kevin - <span>Software Engineering Student</span></h1>
    </div>
    <Nav @showRightPage="emitPage" />
  </header>
</template>

<style scoped>

header {
  background-image: url('/src/assets/css/media/view-3d-modern-abstract-sphere-art.jpg');
  background-size: cover;
  background-position: top;
  padding: 1rem 2rem;
  border-radius: 10rem;
  margin: 1rem 0;
  display: flex;
  justify-content: space-between;
  align-items: center;
  left: 0;
  z-index: 100;
}

h1 {
  font-family: 'Playwrite GB S', sans-serif;
  font-size: 1.5rem;
  white-space: nowrap;
  transition: transform 0.3s ease;
}

h1:hover {
  transform: translateY(-0.2rem);
}

.h1 {
  display: flex;
  align-items: center;
  cursor: pointer;
}

.circle {
  width: 2rem;
  height: 2rem;
  background-color: lightpink;
  border-radius: 50%;
  margin-right: 10px;
}



@media (max-width: 900px) {
  header {
    flex-direction: column;
    padding: 1rem;
    border-radius: 2rem;
    text-align: center;
  }

  .h1 {
    margin-bottom: 1rem;
    flex-direction: column;
  }

  h1 {
    font-size: 1.25rem;
    white-space: normal;
    text-align: center;
  }

  .circle {
    margin: 0 auto 10px;
  }
}

@media (max-width: 1470px) {
  h1 {
    font-size: 1rem;
  }

  .circle {
    width: 1.5rem;
    height: 1.5rem;
  }
}
</style>
