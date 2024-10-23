<script>
export default {
  name: "Nav"
  ,
  methods: {
    handleClick(item) {
      this.$emit("showRightPage", item)
    }
  }
}
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
}

li {
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
</style>