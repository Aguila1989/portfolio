<script>
import BlogCard from "@/components/subPages/blog/BlogCard.vue";

export default {
  name: "Blog",
  components: {BlogCard},
  mounted() {
    window.scrollTo(0, 0);
  }
}
</script>

<template>
  <h1>Blog</h1>
  <section class="blog">
    <BlogCard title="Tech and Meet AI: The reality behind the hype" date="2024-11-21"
              :paragraphs="[
              {description: 'On November 21, 2024, I attended a fascinating presentation by ir. Wim Delvaux. The event was scheduled to start at 6:30 PM but, due to a misunderstanding, it only began at 8:00 PM. Despite the delay, the insights shared made it well worth the wait.'},
              {description: 'The presentation explored the essence of intelligence and how AI attempts to replicate human cognitive processes like observing, learning, reasoning, problem-solving, and language use. Delvaux elaborated on two primary approaches to AI: bottom-up (connectionist), which mimics biological systems using neural networks, and top-down (symbolic), which relies on logical structures like knowledge graphs and databases.'},
              {description: 'He also highlighted the societal impact of AI, emphasizing its transformative potential alongside critical risks, such as overhyped promises and ethical concerns. Notably, he discussed the importance of EU regulations to ensure transparency, mitigate risks, and safeguard public interests in this rapidly evolving domain.'},
              {description: 'This event served as a reminder that while AI offers incredible possibilities, it demands careful scrutiny and responsible implementation to avoid pitfalls.'},
              ]"
              sourceImageRight="src/assets/images/ai de realiteit achter de hype.jpg" imageRightAlt="TuxTalk" />

    <BlogCard title="Hackathon Hack the Future" date="2022-11-19"
              :paragraphs="[
              {description: 'On November 19, 2024, I had the incredible opportunity to participate in the Hackathon Hack the Future, an event designed to push the boundaries of creativity and technical skills. <br>Together with my teammate Clint, we embarked on a thrilling journey to develop a program for astronaut selection using the Solid framework.'},
              {description: 'The project aimed to streamline the astronaut selection process by creating dynamic challenges, maintaining a real-time leaderboard, and incorporating a robust search feature. Although we didn’t take home a prize, the experience was both rewarding and deeply enriching.'},
              {description: 'Our day began with an introduction to the hackathon’s theme, which encouraged us to think outside the box while solving real-world problems. After brainstorming ideas, we decided to focus on the astronaut selection program, given its unique challenges and scope for innovation. <br>The Solid framework proved to be an exciting tool, offering a decentralized approach to managing data and fostering privacy, a key consideration in scenarios like astronaut training.<br> Throughout the day, Clint and I collaborated closely, tackling obstacles and refining our application to make it as efficient and user-friendly as possible.'},
              {description: 'The event itself was exceptionally well-organized, reflecting the thoughtful planning of the organizers. Delicious meals and refreshing drinks kept our energy high, while generous goodie bags added a touch of excitement to the day. <br>Every detail seemed tailored to ensure participants had everything they needed to succeed, fostering an atmosphere of motivation and camaraderie. <br>During breaks, we took the opportunity to explore a nearby zoo, which provided an interesting diversion. However, our enjoyment was tempered by the small enclosures for the animals, which left us feeling a mix of fascination and sadness.'},
              {description: 'Despite not winning, the hackathon offered invaluable lessons and unforgettable moments. We honed our technical skills, learned to think critically under pressure, and deepened our understanding of innovative frameworks like Solid. <br>Most importantly, the event reinforced the joy of creating something meaningful while collaborating with like-minded individuals. <br>The inspiring talks and interactions with other participants further enriched the experience, sparking ideas and new perspectives.'}
              ]"
              sourceImageLeft="src/assets/images/hack the future.jpg"
              imageLeftAlt="baserow" />

    <BlogCard title="Tech and Meet TuxTalk" date="2024-10-29"
              :paragraphs="[
              {description: 'On October 29, we attended an insightful Linux meetup, exploring the newest advancements and trends in the Linux ecosystem. Here’s a look at the main highlights from the discussions:'},
              {description: '&emsp;1. Ubuntu 24.10 – Launched on October 10, Ubuntu 24.10, also known as “Oracular Oriole,” arrived with Linux kernel 6.11, GNOME 47, and a refreshed installer using Flutter. <br>This release is supported for nine months, providing a stable bridge to the upcoming Ubuntu 25.04 next year.'},
              {description: '&emsp;2. GNOME 47.1 – This update focuses on accessibility, with improved display scaling and optimized shortcuts. <br>The goal is a smoother user experience, particularly across devices with varying screen sizes.'},
              {description: '&emsp;3. CachyOS Update – The latest version of this Arch-based distro optimizes performance for AMD hardware, offering faster boot times and new configurations, especially for newer AMD CPUs.'},
              {description: '&emsp;4. System76’s Thelio Astra – System76’s latest ARM64-powered desktop model targets developers and researchers needing high-performance, Linux-specific hardware with flexibility and power.'},
              {description: 'We searched for Tech and Meets online and came across this one but honestly it was a bit disappointing...'},
              ]"
              sourceImageRight="src/assets/images/tuxTalk.jpg" imageRightAlt="TuxTalk" />

    <BlogCard title="Tech and Meet BaseRow" date="2022-10-22"
              :paragraphs="[
              {description: 'October 22st, I attended a tech meet at Howest that featured a presentation on Baserow, an open-source database software. The speaker, who commenced at 19:00 and finished at 20:00, introduced Baserow as a versatile platform that simplifies database management.'},
              {description: 'He emphasized that with Baserow, you only pay for a license once, and you are ready to go.'},
              {description: 'Baserow is marketed as being more user-friendly than MySQL, offering built-in authentication and an extensive set of functions, such as roll-up formulas and built-in templates for easy database creation.'},
              {description: 'One standout feature is the ability to create views, including bread views, without writing complex queries. <br>The software also offers a graphical interface to manage your database, allowing users to collaborate by tagging colleagues directly in the app, eliminating the need for external tools like Teams.'},
              {description: 'As an admin, you also have access to an audit log, which tracks every action taken. Baserow includes a task management system and dashboards that provide insights without requiring users to sift through spreadsheets.'},
              {description: 'The no-code builder makes it easy to create and manage a responsive front end without needing to write a single line. <br> Users can even automate API development through visual programming tools and predefined blocks.'},
              {description: 'The speaker showcased practical examples of Baserow’s capabilities, including a smoothie ordering system and a city tour app that highlights key locations on a map. <br> He emphasized that since starting with Baserow in February, the platform has evolved rapidly, offering faster development cycles for low- or no-code applications, though with some limitations.'},
              {description: 'After the presentation, we gathered in the A-building for drinks, continuing discussions until 22:00 in a relaxed and informal setting. It was a great evening of learning, networking, and sharing ideas.'}
              ]"
              sourceImageLeft="src/assets/images/baserow.jpg"
              imageLeftAlt="baserow" />
  </section>
</template>

<style scoped>
  h1{
    font-family: 'Playwrite GB S', sans-serif;
    margin-top: 5rem;
    text-align: center;
  }
  .blog{
    padding:2rem;
  }

  @media (max-width: 1300px) {
    .blog{
      padding: 0;
    }
  }
</style>