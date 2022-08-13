<template>
  <body class="image h-screen bg-center bg-no-repeat bg-cover">
    <li class="list-none flex items-center gap-5 p-4">
      <ul>
        <a href="https://github.com/Mahadfarooq10">
          <button>
            <Github :width="2.5" :height="2.5" class="enlarge" />
          </button>
        </a>
      </ul>
      <ul>
        <a href="https://www.linkedin.com/in/mahad-farooq-2004a71b3/">
          <button>
            <Linkedin :width="2.5" :height="2.5" class="enlarge" />
          </button>
        </a>
      </ul>
      <ul>
        <a href="mailto: mahadfarooq1998@gmail.com">
          <button>
            <At :width="2.8" :height="2.8" class="enlarge" />
          </button>
        </a>
      </ul>
      <ul>
        <a href="resume.pdf" download="resume.pdf">
          <button>
            <Resume :width="2.3" :height="2.3" class="enlarge" />
          </button>
        </a>
      </ul>
    </li>
    <Description />
  </body>
</template>

<script setup lang="ts">
import Github from "../components/icons/github.vue";
import Linkedin from "../components/icons/linkedin.vue";
import At from "../components/icons/at.vue";
import Resume from "../components/icons/resume.vue";
import Description from "../components/Description.vue";

</script>

<style scoped>
.image {
  background-image: url("../assets/background.jpg");
}
.enlarge:hover {
  transform: scale(1.25);
}
.enlarge {
  transition: all 0.5s;
  transform-origin: 50% 50%;
}
</style>
