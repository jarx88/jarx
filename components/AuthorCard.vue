<template>
  <div class="md:fixed">
    <div class="md:block flex justify-center items-center">
      <nuxt-img
        :src="siteMetadata.author_image"
        loading="lazy"
        alt="me"
        class="shadow-xl md:h-60 md:w-60 h-40 w-40 rounded-full author-image"
      />
      <div class="mb-2 mx-7 mt-4 justify-center items-center">
        <h1
          class="md:text-3xl text-2xl text-gray-800 font-bold dark:text-blue-100"
        >
          {{ siteMetadata.author }}
        </h1>
        <div class="md:text-lg text-gray-600 dark:text-blue-100">
          {{ siteMetadata.position }}
        </div>
        <a
          :href="`mailto:${siteMetadata.email}`"
          class="text-gray-600 md:hidden mt-1 dark:text-blue-100"
        >
          {{ siteMetadata.email }}
        </a>
        <a
          href="tel:532541533"
          class="text-gray-600 md:hidden mt-1 dark:text-blue-100"
        >
          {{ siteMetadata.phone }}
        </a>
      </div>
    </div>

    <div class="mx-7 hidden md:block">
      <div class="my-2 text-gray-600 flex dark:text-blue-100">
        <Mail />
        <a :href="`mailto:${siteMetadata.email}`"> {{ siteMetadata.email }}</a>
      </div>
      <div class="my-2 text-gray-600 flex dark:text-blue-100">
        <Glob />
        <p>{{ siteMetadata.location }}</p>
      </div>
      <!-- <div class="my-2 text-gray-600 flex dark:text-blue-200">
        <Github />
        <a :href="siteMetadata.github"> {{ siteMetadata.githubUser }}</a>
      </div> -->
      <div class="my-2 text-gray-600 flex dark:text-blue-200 phone">
        <Phone />
        {{ siteMetadata.phone }}
      </div>
      <div class="my-2 text-gray-600 flex dark:text-blue-200 phone">
        <p />
      </div>
      <div class="my-2 text-gray-600 flex dark:text-blue-200">
        <p>Blog:</p></div>
        <div class="my-2 text-gray-600 flex dark:text-blue-200">
        <a href="https://blog.jarx.pl">
          <nuxt-img
        :src="siteMetadata.blog_image"
        loading="lazy"
        alt="blog"
        class="blog-image"
          />
        </a>
      </div>
    </div>
  </div>
</template>

<script>
import Mail from "../assets/icon/mail.svg?inline";
import Glob from "../assets/icon/glob.svg?inline";
import Github from "../assets/icon/github_new.svg?inline";
import Phone from "../assets/icon/phone.svg?inline";
import blog from "../assets/blog.png";
import siteMetaInfo from "@/data/sitemetainfo";
export default {
  components: { Mail, Glob, Github,Phone,blog },
  data: () => {
    return {
      siteMetadata: siteMetaInfo,
    };
  },
};
</script>
