<script>
import BlogCard from "@/components/subPages/blog/BlogCard.vue";

export default {
  name: "Blog",
  components: {BlogCard}
}
</script>

<template>
  <h1>Blog</h1>
  <div class="blog">
    <BlogCard title="Blog 1" date="2021-01-01" description="This is the first blog post" sourceImageLeft="src/assets/images/battleship.jpg" imageLeftAlt="lala" />
    <BlogCard title="Blog 2" date="2021-01-02" description="This is the second blog post" sourceImageRight="src/assets/images/battleship.jpg" imageRightAlt="lala" />
    <BlogCard title="Tech and Meet BaseRow" date="2022-10-22"
              description="On October 22st, I attended a tech meet at Howest that featured a presentation on Baserow, an open-source database software. The speaker, who commenced at 19:00 and finished at 20:00, introduced Baserow as a versatile platform that simplifies database management. <br>
              He emphasized that with Baserow, you only pay for a license once, and you're ready to go.<br><br>
              Baserow is marketed as being more user-friendly than MySQL, offering built-in authentication and an extensive set of functions, such as roll-up formulas and built-in templates for easy database creation. <br>
              One standout feature is the ability to create views, including 'bread views,' without writing complex queries. <br>
              The software also offers a graphical interface to manage your database, allowing users to collaborate by tagging colleagues directly in the app, eliminating the need for external tools like Teams.<br><br>
              As an admin, you also have access to an audit log, which tracks every action taken. Baserow includes a task management system and dashboards that provide insights without requiring users to sift through spreadsheets. <br>
              The no-code builder makes it easy to create and manage a responsive front end without needing to write a single line. <br>
              Users can even automate API development through visual programming tools and predefined blocks.<br><br>
              The speaker showcased practical examples of Baserow’s capabilities, including a smoothie ordering system and a city tour app that highlights key locations on a map. <br>
              He emphasized that since starting with Baserow in February, the platform has evolved rapidly, offering faster development cycles for low- or no-code applications, though with some limitations.<br><br>
              After the presentation, we gathered in the A-building for drinks, continuing discussions until 22:00 in a relaxed and informal setting. It was a great evening of learning, networking, and sharing ideas."
              sourceImageLeft="src/assets/images/baserow.jpg"
              imageLeftAlt="baserow" />
  </div>
</template>

<style scoped>
  h1{
    font-family: 'Playwrite GB S', sans-serif;
    margin-top: 5rem;
  }
  .blog{
    padding:2rem;
  }

  @media (max-width: 768px) {
    .blog{
      padding: 0;
    }
  }
</style>