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
  <div class="resume-card">
    <h2>{{ title }}</h2>
    <div v-for="(section, index) in sections" :key="index">
      <h3 v-if="section.title">{{ section.title }}</h3>
      <p v-if="section.text">{{ section.text }}</p>
    </div>
  </div>
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
}

h2 {
  margin-bottom: 1.5rem;
}

h3 {
  margin-bottom: 0.5rem;
  font-size: 1.5rem;
}

p {
  font-size: 1.25rem;
  margin-bottom: 1rem;
}

/* Responsive adjustments */
@media (max-width: 768px) {
  .resume-card {
    width: 100%;
    padding: 2rem;
    margin-left: 0;
    margin-right: 0;
  }

  h2 {
    font-size: 1.75rem;
  }

  h3 {
    font-size: 1.25rem;
  }

  p {
    font-size: 1rem;
  }
}
</style>
