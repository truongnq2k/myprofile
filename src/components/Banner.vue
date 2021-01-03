<template>
  <section class="my-5">
    <div class="container">
      <div class="p-4 border">
        <h1>
          Progress on my <span class="text-success">projects</span> in 2021
        </h1>
        <p class="lead">My Projects will work in 2021:</p>
        <ul>
          <li v-for="project in projects" :key="project.name">
            {{ project.name }}
          </li>
        </ul>
        <hr />
        <p>
          All my projects will be uploaded to github and gitlab:
          <a href="https://github.com/truongnq2k">Github</a> |
          <a href="https://gitlab.com/truongnq2k">Gitlab</a>
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        { name: "Elearning Full Stack" },
        { name: "Library System" },
        { name: "Some project using microservices" },
      ],
    };
  },
};
</script>

<style>
</style>