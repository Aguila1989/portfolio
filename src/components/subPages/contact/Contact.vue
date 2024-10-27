<script>
export default {
  name: "Contact",
  mounted() {
    window.scrollTo(0, 0);
  }
}
</script>

<template>
  <h1>Contact</h1>
  <div class="contact-info">
    <section class="contact-container">
      <h2>Contact Information</h2>
      <h3>Email:</h3>
      <p class="mail"><a href="mailto:k.demeulenaere@hotmail.com">k.demeulenaere@hotmail.com</a></p>
      <h3>Phone:</h3>
      <p class="phone"><a href="https://wa.me/32474761753" target="_blank">+32(0)474/76.17.53</a></p>
      <h3>LinkedIn:</h3>
      <p class="linked"><a href="https://www.linkedin.com/in/kevin-demeulenaere-63563b87?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app" target="_blank">My LinkedIn Profile</a></p>
    </section>
  </div>
</template>

<style scoped>
.contact-info {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 70vh;
}

.contact-container {
  opacity: 0.8;
  background-color: #ffffff;
  border: 0.05rem solid lightgrey;
  padding: 3rem 4rem;
  border-radius: 1rem;
  box-shadow: 10px 10px 22px -15px rgba(0, 0, 0, 0.5);
  max-width: 600px;
  width: 90%;
}

h1 {
  font-family: 'Playwrite GB S', sans-serif;
  margin-top: 5rem;
  text-align: center;
}

h2 {
  font-family: 'Playwrite GB S', sans-serif;
  font-size: 2rem;
  margin-bottom: 2rem;
  text-decoration: underline;
  text-align: center;
}

h3 {
  font-family: 'Playwrite GB S', sans-serif;
  font-size: 1.5rem;
  margin-bottom: 0.5rem;
}

p {
  font-family: 'Lato', serif;
  font-size: 1rem;
  margin-bottom: 1rem;
  padding: 0.5rem;
  border: 1px solid lightgray;
  border-radius: 0.5rem;
  width: fit-content;
  cursor: pointer;
  box-shadow: 5px 5px 15px -5px rgba(0, 0, 0, 0.75);
  transition: background-color 0.3s ease;
  line-height: 170%;
}

.mail, .phone, .linked {
  transition: transform 0.3s ease;
}

.mail:hover, .phone:hover, .linked:hover {
  background-color: rgba(244, 214, 96, 0.98);
  transform: translateY(-0.15rem);
}

.mail {
  background-color: rgba(250, 197, 197, 0.99);
}

.phone {
  background-color: lightblue;
}

.linked {
  background-color: #9af19a;
}

a {
  text-decoration: none;
  color: black;
}

@media (max-width: 900px) {



  .contact-container {
    display: flex;
    flex-direction: column;
    padding: 2rem 3rem;
    justify-content: center;
    align-items: center;
    width: 100%;
  }

  h1, h2, h3, p {
    text-align: center;
  }


}
</style>
