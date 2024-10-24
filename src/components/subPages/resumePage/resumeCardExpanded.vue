<script>
export default {
  name: "ResumeCardExpanded",
  props: {
    title: {
      type: String,
      required: true
    },
    sections: {
      type: Array,
      required: true,
      default: () => []
    }
  }
}
</script>

<template>
  <article class="resume-card">
    <h2>{{ title }}</h2>
    <div v-for="(section, index) in sections" :key="index">
      <h3 v-if="section.title">{{ section.title }}</h3>
      <p v-if="section.text">{{ section.text }}</p>
    </div>
  </article>
</template>

<style scoped>

.resume-card {
  border: 0.05rem solid lightgrey;
  padding: 3rem 6rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  width: 45%;
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
  margin-bottom: 1.5rem;
}

h3 {
  font-family: 'Lato', serif;
  margin-bottom: 0.5rem;
  font-size: 1.5rem;
}

p {
  font-family: 'Lato', serif;
  font-size: 1.25rem;
  margin-bottom: 1rem;
}

@media (max-width: 900px) {
  .resume-card {
    width: 100%;
    padding: 2rem;
    margin-left: 0;
    margin-right: 0;
  }

}
</style>
