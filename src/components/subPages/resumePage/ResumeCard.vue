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
  <div class="resume-card">
    <h2>{{title}}</h2>
    <div class="list" v-html="list"></div>
  </div>
</template>

<style scoped>
.resume-card{
  border: 0.05rem solid lightgrey;
  padding: 3rem 6rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  width: 45%;
  margin-bottom: 2rem;
  margin-left: 1rem;
  margin-right: 1rem;
}
h2{
  margin-bottom: 1.5rem;
}

.list{
  font-size: 1.25rem;
}

</style>