<script>
export default {
  name: "Contact"
}
</script>

<template>
  <h1>Contact</h1>
  <div class="contact-info">
    <div class="contact-container">
<h2>CONTACT INFORMATION</h2>
  <h3>Email:</h3>
  <p class="mail"><a href="mailto:k.demeulenaere@hotmail.com">k.demeulenaere@hotmail.com</a></p>
  <h3>Phone:</h3>
  <p class="phone"><a href="https://wa.me/32474761753" target="_blank">+32(0)474/76.17.53</a></p>
  <h3>LinkedIn:</h3>
      <p class="linked"><a href="https://www.linkedin.com/in/kevin-demeulenaere-63563b87?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app " target="_blank">My LinkedIn Profile</a></p>
  </div>
  </div>
</template>

<style scoped>
  .contact-info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 70vh;
  }

  .contact-container{

    opacity: 0.8;
    background-color: #ffffff;
    border: 0.05rem solid lightgrey;
    padding: 3rem 6rem;
    border-radius: 1rem;
    box-shadow: 10px 10px 22px -15px rgba(0,0,0,1);
  }

  h1{
    font-family: 'Playwrite GB S', sans-serif;
    margin-top: 5rem;
  }

  h2{
    font-family: 'Playwrite GB S', sans-serif;
    font-size: 2rem;
    margin-bottom: 2rem;
    text-decoration: underline;
  }

  h3{
    font-family: 'Playwrite GB S', sans-serif;
    font-size: 1.5rem;
    margin-bottom: 0.5rem;
  }

  p{
    font-family: 'Lato', serif;
    font-size: 1rem;
    margin-bottom: 1rem;
    padding: 0.5rem;
    border: 1px solid lightgray;
    border-radius: 0.5rem;
    width: fit-content;
    cursor: pointer;
    box-shadow: 5px 5px 15px -5px rgba(0,0,0,0.75);
  }

.mail:hover, .phone:hover, .linked:hover{
    background-color: rgba(244, 214, 96, 0.98);
  }
.mail{
  background-color: rgba(250, 197, 197, 0.99);
}
.phone{
  background-color: lightblue;
}
.linked{
  background-color: #9af19a;
}

  a{
    text-decoration: none;
    color: black;
  }

</style>