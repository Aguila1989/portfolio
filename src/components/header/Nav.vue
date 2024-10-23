<script>
export default {
  name: "Nav",
  methods: {
    handleClick(item) {
      this.$emit("showRightPage", item);
    }
  }
};
</script>

<template>
  <ul>
    <li @click="handleClick('about')">About me</li>
    <li @click="handleClick('resume')">Resume</li>
    <li @click="handleClick('portfolio')">My Work</li>
    <li @click="handleClick('blog')">Blog</li>
    <li @click="handleClick('contact')">Contact</li>
  </ul>
</template>

<style scoped>
ul {
  display: flex;
  justify-content: space-between;
  list-style: none;
  padding: 0;
  margin: 0;
}

li {
  font-family: 'Playwrite GB S', sans-serif;
  border-right: 1px solid black;
  padding: 0.5rem 1rem;
  font-size: 1.25rem;
}

li:last-child {
  border-right: none;
}

li:hover {
  background-color: lightpink;
  cursor: pointer;
  box-shadow: 10px 10px 20px -14px blue;
}

@media (max-width: 1300px) {
  ul {
    flex-direction: column;
    align-items: center;
  }

  li {
    border-right: none;
    border-bottom: 1px solid black;
    width: 100%;
    text-align: center;
  }

  li:last-child {
    border-bottom: none;
  }
}

@media (max-width: 650px) {
  li {
    font-size: 1rem;
    padding: 0.5rem 0.75rem;
  }
}
</style>
