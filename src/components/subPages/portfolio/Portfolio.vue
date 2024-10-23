<script>
import PortfolioCard from "@/components/subPages/portfolio/PortfolioCard.vue";

export default {
  name: "Portfolio",
  components: {PortfolioCard},
  mounted() {
    window.scrollTo(0, 0);
  }
}
</script>

<template>
  <h1>My Work</h1>
  <div class="portfolio">
    <PortfolioCard title="Portfolio" link-description="Link to GitHub" link="https://github.com/Aguila1989/portfolio" alt="portfoliio"
                   source="/src/assets/images/portfolio.jpg"
                   text="I decided to make a portfolio in Vue.js. <br>
                   I added all my previous projects, including this one, to the portfolio. <br>
                    I also added a blog page where I can write about my experiences and projects, and an about me and contact page to give visitors a better idea of who I am and what I do. <br>
                    I tried to build the portfolio as user-friendly as possible, with a clean design and easy navigation, also spliiting up the code in the right components <br>" />
    <PortfolioCard title="RecipEasy" link-description="Link to GitHub" link="https://github.com/Aguila1989/RecipEasy" alt="RecipEasy"
                   source="/src/assets/images/recipeasy.png"
                   text='For a school assignment, our team developed RecipEasy, a native Android app using Kotlin and Jetpack Compose.<br>
                    The app simplifies meal prep by offering a curated list of recipes from a third-party API, with each recipe providing detailed instructions, ingredients, and nutritional information.<br>
                     We also added a pantry feature, allowing users to track available ingredients and find recipes based on what they have on hand, making meal prep more efficient.<br>
                      The app includes filters for cuisines and dietary needs, along with push notifications for a "recipe of the day" to keep users engaged. <br>
                      A calendar function helps users plan meals, while a shopping list feature makes it easy to add ingredients directly from recipes. <br>
                      This project was our first with Kotlin, and our Java background helped us transition smoothly, giving us valuable experience in modern mobile app development and enhancing our skills in creating user-friendly applications.'/>

    <PortfolioCard title="Magic The Gathering" link-description="Link to GitHub" link="https://github.com/Aguila1989/magic-the-gahteric" alt="Magic The Gathering"
                   source="/src/assets/images/mtg.png"
                   text="In this Magic: The Gathering project, I built a web app using .NET for the backend and Blazor for the frontend, allowing users to build and manage decks by saving cards to personalized collections. <br>
                   We used Microsoft SQL Server to store and retrieve card data, making it easy for users to search for cards by name, type, or color. <br>
                   A major focus was learning how to write APIs in .NET, where I explored minimal APIs, WebAPIs, and GraphQL, gaining valuable experience in API development. <br>
                   On the frontend, Blazor provided a dynamic user interface, while MongoDB was integrated for scalable storage of user data and deck collections. <br>
                   This project was a rewarding culmination of my semester's learning, combining API creation, frontend integration, and database management. <br>
                   It reinforced my skills in the .NET ecosystem and problem-solving, preparing me for future development projects."/>

    <PortfolioCard title="Adria" link-description="Link to GitHub" link="https://github.com/Aguila1989/adria" alt="Adria"
                   source="/src/assets/images/adria.png"
                   text="For a school project, my team and I created AdraMed, a startup concept aimed at rebuilding the world after the Global Disaster of 2064. <br>
                   The assignment challenged us to envision innovative solutions for a post-apocalyptic future, and we focused on healthcare with our flagship product, ResQ. <br>
                   ResQ is a personal medical assistant powered by advanced AI to monitor health, provide real-time diagnoses, and offer wellness plans for a better quality of life. <br>
                   The project also included futuristic features like space travel preparation and emergency response for explorers and colonists. <br>
                   Our goal was to create a product that not only saves lives but also enhances them, making healthcare accessible and effective for all. <br>
                   This project allowed us to explore how technology can play a vital role in rebuilding society."/>
    <PortfolioCard title="Brandy" link-description="Link to website" link="https://play.brandygame.eu/" alt="Brandy"
                   source="/src/assets/images/brandy.png"
                   text="At the end of the school year, I was selected for an international project in Valencia called Brandy, <br>
                   a business simulation game co-funded by the Erasmus program. Over the course of a week, we worked in teams, tackling daily challenges and competing for awards. <br>
                   My team worked on the final version of the game, using a Svelte frontend and Laravel backend, which gave us the chance to learn Svelte while improving the platform. <br>
                   The biggest challenge was navigating the existing codebase and implementing feedback from students and teachers. Despite the initial difficulties,
                   we successfully added new features and fixed bugs, making the project a rewarding learning experience. <br>
                   It improved my technical skills and showed me the importance of teamwork in a real-world setting."/>

    <PortfolioCard title="BattleShip" link-description="Link to GitHub" link="https://github.com/Aguila1989/battleship" alt="BattleShip"
                   source="/src/assets/images/battleship.jpg"
                   text="One of my most exciting first-year projects was transforming the classic Battleship board game into a fully functional website. <br>
                   We built the backend using Java and the frontend with JavaScript, HTML, and CSS, adding modes like Salvo and move-and-shoot to keep the gameplay fresh. <br>
                   The frontend allowed players to customize themes, sound effects, and animations while navigating easily to challenge friends or random opponents. <br>
                   Real-time updates on ship status and strategic shot tracking made for an engaging experience, with a satisfying conclusion at the end of each match. <br>
                   Building the backend taught us the importance of clean architecture and adhering to API specifications, making this our first experience with complex full-stack development. <br>
                   In the end, we were proud of our work, as it exceeded our expectations and gave us the confidence to tackle even bigger challenges."/>
</div>
</template>
<style scoped>

h1 {
  font-family: 'Playwrite GB S', sans-serif;
  margin-top: 5rem;
  text-align: center;
}

.portfolio {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  padding: 2rem;
}

@media (max-width: 900px) {

  .portfolio {
    padding: 0;
  }
}
</style>