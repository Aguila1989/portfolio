<script>
export default {
  name: "BlogCard"
  ,
  props: {
    title: {
      type: String,
      required: true
    },
    date: {
      type: String,
      required: true
    },
    description: {
      type: String,
      required: true
    },
    sourceImageLeft: {
      type: String,
      required: false
    },
    imageLeftAlt: {
      type: String,
      required: false
    },
    sourceImageRight: {
      type: String,
      required: false
    },
    imageRightAlt: {
      type: String,
      required: false
    }
  }
}
</script>

<template>
  <div class="blog-card">
    <div class="title">
    <h2>{{title}}</h2>
    <p>{{date}}</p>
    </div>
    <div class="blog-description">
      <img v-if="sourceImageLeft" :src="sourceImageLeft" alt="{{imageLeftAlt}}">
    <p class="description" v-html="description"></p>
      <img v-if="sourceImageRight" :src="sourceImageRight" alt="{{imageRightAlt}}">
    </div>
  </div>
</template>

<style scoped>
.title{
  display: flex;
  justify-content: space-between;
  margin-bottom: 1.5rem;
}

.blog-card{
  background-color: #ffffff;
  opacity: 0.8;
  border: 0.05rem solid lightgrey;
  padding: 3rem 6rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  margin-bottom: 2rem;
  margin-left: 1rem;
  margin-right: 1rem;
}

.blog-description
{
  display: flex;
  justify-content: space-between;
  gap: 2rem;
}

img{
  max-width: 20rem;
  min-width: 20rem;
  max-height: 20rem;
  min-height: 20rem;
  border-radius: 2rem;
align-self: center;
}
.description{
  font-size: 1.25rem;
}
</style>