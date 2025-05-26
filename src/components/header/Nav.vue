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
    <li class="li-left" @click="handleClick('about')">About me</li>
    <li class="li-mid" @click="handleClick('resume')">Resume</li>
    <li class="li-mid" @click="handleClick('portfolio')">My Work</li>
    <li class="li-right" @click="handleClick('blog')">Blog</li>
    <li class="li-right" @click="handleClick('contact')">Contact</li>
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
  transition: transform 0.3s ease;
}

li:last-child {
  border-right: none;
}

.li-mid:hover {
  background-color: #fdfbf4;
  box-shadow: 10px 10px 20px -14px lightgreen;
}

.li-left:hover {
  background-color: #fef4e7;
  box-shadow: 10px 10px 20px -14px lightgreen;
}

.li-right:hover {
  background-color: #c7e4d6;
  box-shadow: 10px 10px 20px -14px lightskyblue;
}

li:hover {
  cursor: pointer;
  transform: translateY(-0.2rem);
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

  .li-mid:hover, .li-left:hover {
    background-color: #c7e4d6;
    box-shadow: 10px 10px 20px -14px lightskyblue;
  }

  .li-right:hover {
    background-color: #fef4e7;
    box-shadow: 10px 10px 20px -14px #c7e4d6;
  }

  li:last-child {
    border-bottom: none;
  }
}

@media (max-width: 900px) {
  li {
    font-size: 1rem;
    padding: 0.5rem 0.75rem;
  }
  .li-mid:hover , .li-left:hover, .li-right:hover {
    background-color: #fef4e7;
    box-shadow: 10px 10px 20px -14px lightskyblue;
  }
}
</style>
