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
        <img src="/src/assets/images/Screenshot%202024-10-21%20235517.png" alt="itsa me">
        <div>
        <h2>Hi there, I'm Kevin</h2>
          <p>I'm a last year student Bachelor Applied Informatics with a specialization towards Software Engineering at the university of Howest Bruges.<br>
          As a dedicated developer, I’m enthusiastic about learning new technologies, collaborating with teams,
          and thriving in an agile environment. I have successfully completed a range of projects, from web applications to software systems,
          and I am continually seeking opportunities to enhance my skills and grow as a professional.
        </p>
        </div>
      </div>
          <div class="photo-and-text">
            <div>
          <h2>Future Goals</h2>
          <p>As I continue my journey in Software Engineering, my ultimate goal is to achieve financial freedom while doing what I love. I aspire to explore the world, discovering new cultures and places like Antarctica, Norway and Iceland, which have always been dream destinations of mine. Professionally, I aim to grow as a front-end developer, mastering modern technologies and contributing to innovative projects that make a positive impact.</p>
            </div>
            <img src="/src/assets/images/explore.jpg" alt="explore">
          </div>
          <div class="photo-and-text">
            <img src="/src/assets/images/hobbies.jpg" alt="hobbies">
            <div>
          <h2>Hobbies
          </h2>
          <p>When I'm not coding, I enjoy spending time with my friends and family, wall climbing, going to the gym, and watching movies. I also love to travel and explore new places, and I'm always up for an adventure. I'm passionate about music and play the piano in my free time.
          </p>
        </div>
      </div>
          <div class="photo-and-text">
            <div>
          <h2>Favorite Quote
          </h2>
          <p>
            "Compare yourself to who you were yesterday, not to who someone else is today." – Jordan Peterson
          </p>
    </div>
            <img src="/src/assets/images/jordan.jpg" alt="jordan peterson">
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
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 2rem;
  min-height: 70vh;
}

h1 {
  font-family: 'Playwrite GB S', sans-serif;
  margin-top: 5rem;
  margin-bottom: 2rem;
  text-align: center;
}
h2{
  margin: 1rem 0;
}

.photo-and-text {
  display: flex;
  background-color: #ffffff;
  align-items: center;
  justify-content: center;
  font-size: 1.25rem;
  border: 0.05rem solid lightgrey;
  min-height: 30rem;
  min-width: 60vw;
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
