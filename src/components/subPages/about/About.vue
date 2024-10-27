<script>
export default {
  name: "About",
  mounted() {
    window.scrollTo(0, 0);
  }
};
</script>

<template>
  <article class="about-me">
    <h1>About me</h1>
    <div class="me">
      <div class="photo-and-text">
        <img src="/src/assets/images/Screenshot%202024-10-21%20235517.png" alt="">
        <div>
        <p>Hi there, I'm Kevin</p>
          <p>I'm a last year student Bachelor Applied Informatics with a specialization towards Software Engineering at the university of Howest Bruges.<br>
          As a dedicated developer, I’m enthusiastic about learning new technologies, collaborating with teams,
          and thriving in an agile environment. I have successfully completed a range of projects, from web applications to software systems,
          and I am continually seeking opportunities to enhance my skills and grow as a professional.
        </p>
        </div>
      </div>
    </div>
  </article>
</template>

<style scoped>
img {
  border-radius: 55rem;
  width: 20rem;
  height: 20rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  transition: transform 0.3s ease;
}

img:hover {
  transform: translateY(-0.2rem);
}

.me {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 2rem;
  min-height: 70vh;
}

h1 {
  font-family: 'Playwrite GB S', sans-serif;
  margin-top: 5rem;
  text-align: center;
}

.photo-and-text {
  display: flex;
  background-color: #ffffff;
  align-items: center;
  font-size: 1.25rem;
  border: 0.05rem solid lightgrey;
  min-height: 30rem;
  padding: 2rem 4rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 1);
  gap: 4rem;
  opacity: 0.9;
}

p {
  font-family: 'Lato', serif;
  width: 40rem;
  transition: transform 0.3s ease;
  margin-bottom: 1rem;
  line-height: 170%;
}

p:hover {
  transform: translateY(-0.2rem);
}

/* Responsive Styles */
@media (max-width: 1024px) {
  p {
    width: 30rem;
  }

  .photo-and-text {
    flex-direction: column;
    text-align: center;
    padding: 2rem;
    gap: 2rem;
  }

  img {
    width: 15rem;
    height: 15rem;
  }
}

@media (max-width: 1100px) {
  p {
    width: 20rem;
    font-size: 1.1rem;
  }

  img {
    width: 12rem;
    height: 12rem;
  }

  .photo-and-text {
    padding: 1.5rem;
  }
}

@media (max-width: 480px) {
  p {
    width: 18rem;
    font-size: 1rem;
  }

  img {
    width: 10rem;
    height: 10rem;
  }

  h1 {
    margin-top: 2rem;
    font-size: 1.5rem;
  }

  .photo-and-text {
    padding: 1rem;
    min-height: auto;
  }
}
</style>
