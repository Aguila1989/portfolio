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