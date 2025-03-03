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
    paragraphs: {
      type: Array,
      required: true,
      default: () => []
    },
    imageRightAlt: {
      type: String,
      required: false
    }
  }
}
</script>

<template>
  <article class="blog-card">
    <div class="title">
      <h2>{{ title }}</h2>
      <p class="date">{{ date }}</p>
    </div>
    <div class="blog-description">
      <img v-if="sourceImageLeft" :src="sourceImageLeft" alt="{{imageLeftAlt}}">
      <div class="paragraphs">
        <div v-for="(paragraph, index) in paragraphs" :key="index">
          <p class="description" v-html="paragraph.description" ></p>
        </div>
      </div>
      <img v-if="sourceImageRight" :src="sourceImageRight" alt="{{imageRightAlt}}">
    </div>
  </article>
</template>

<style scoped>
.title {
  display: flex;
  justify-content: space-between;
  margin-bottom: 1.5rem;
}

.blog-card {
  background-color: #ffffff;
  opacity: 0.8;
  border: 0.05rem solid lightgrey;
  padding: 3rem 6rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  margin-bottom: 2rem;
  margin-left: 1rem;
  margin-right: 1rem;
  transition: transform 0.3s ease;
}

.blog-card:hover {
  transform: translateY(-0.2rem);
}

.blog-description {
  display: flex;
  justify-content: space-between;
  gap: 2rem;
}

h2 {
  font-family: 'Playwrite GB S', sans-serif;
}

.date {
  font-family: 'Playwrite GB S', serif;
}

p {
  font-family: 'Lato', serif;
  line-height: 170%;
  margin-bottom: 1rem;
}

img {
  max-width: 20rem;
  min-width: 20rem;
  max-height: 20rem;
  min-height: 20rem;
  border-radius: 2rem;
}

.paragraphs {
  display: flex;
  flex-direction: column;
}

.description {
  font-size: 1.25rem;
}

@media (max-width: 1150px) {

  .blog-card {
    width: 100%;
    padding: 2rem;
    margin-left: 0;
    margin-right: 0;
  }


  .blog-description {
    flex-direction: column;
    width: 100%;
  }

  img {
    max-width: 15rem;
    min-width: 15rem;
    max-height: 15rem;
    min-height: 15rem;
  }

  @media (max-width: 800px) {
    .title {
      flex-direction: column-reverse;
      width: 100%;
    }
  }
}
</style>