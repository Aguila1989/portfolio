<script>
export default {
  name: "ResumeCard",
  props: {
    title: {
      type: String,
      required: true
    },
    list: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <article class="resume-card">
    <h2>{{ title }}</h2>
    <div class="list" v-html="list"></div>
  </article>
</template>

<style scoped>

.resume-card {
  border: 0.05rem solid lightgrey;
  padding: 3rem 6rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  margin-bottom: 2rem;
  margin-left: 1rem;
  margin-right: 1rem;
  background-color: white;
  transition: transform 0.3s ease;
}

.resume-card:hover {
  transform: translateY(-0.2rem);
}

h2 {
  font-family: 'Playwrite GB S', sans-serif;
  font-size: 1.5rem;
  margin-bottom: 2.5rem;
  text-decoration: underline 1px;
}

p {
  font-family: 'Lato', serif;
  font-size: 1.25rem;
  margin-bottom: 1rem;
  line-height: 170%;
}

.list {
  font-family: 'Lato', serif;
  font-size: 1.25rem;
}

@media (max-width: 900px) {
  .resume-card {
    padding: 2rem;
    margin-left: 0;
    margin-right: 0;
  }

}
</style>
