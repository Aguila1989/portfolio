<script>
export default {
  name: "PortfolioCard",
  props: {
    title: {
      type: String,
      required: true
    },
    text: {
      type: String,
      required: true
    },
    source: {
      type: String,
      required: true
    },
    alt: {
      type: String,
      required: true
    },
    link: {
      type: String,
      required: true
    },
    linkDescription: {
      type: String,
      required: true
    }
  }
}
</script>

<template>
  <div class="portfolio-card">
    <img :src="source" alt="{{alt}}">
    <h2>{{title}}</h2>
    <p v-html="text"></p>
    <p><a :href="link" target='_blank'>{{ linkDescription }}</a></p>
  </div>
</template>

<style scoped>
.portfolio-card{
  display: flex;
  flex-direction: column;
  align-items: start;
  border: 0.05rem solid lightgrey;
  padding: 3rem 6rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  width: 45%;
  margin-bottom: 2rem;
  margin-left: 1rem;
  margin-right: 1rem;
  background-color: #ffffff;
  opacity: 0.8;
}

img{
  align-self: center;
  border-radius: 20rem;
  object-fit: cover;
  width: 20rem;
  height: 20rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  margin-bottom: 2rem;
}

h2{
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

p{
  font-family: 'Lato', serif;
  font-size: 1.25rem;
  margin-bottom: 1rem;
}


@media (max-width: 1300px) {
  .portfolio-card {
    padding: 2rem;
  }

}

@media (max-width: 900px) {
  .portfolio-card {
    width: 100%;
    margin-left: 0;
    margin-right: 0;
  }

  img {
    width: 15rem;
    height: 15rem;
  }
}
</style>