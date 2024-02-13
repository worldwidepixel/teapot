<template>
  <title> I am a teapot. Are you? </title>
  <div class="mainLayout">
    <span class="titleText">{{ error.statusCode }}</span>
    <span>{{ error.message }}</span>

    <div class="spacer" />

    <div class="aboutList">
      <NuxtLink to="https://blurryface.xyz">
        <span class="user"> <img class="userImg" src="https://avatars.githubusercontent.com/blryface"> </span>
      </NuxtLink>
      <NuxtLink to="https://worldwidepixel.ca">
        <span class="user"> <img class="userImg" src="https://avatars.githubusercontent.com/worldwidepixel"> </span>
      </NuxtLink>
    </div>
  </div>
</template>

<style>


  @import url(https://fonts.bunny.net/css?family=inter:100,200,300,400,500,600,700,800,900);

  :root {
    font-family: Inter, Helvetica, sans-serif;
    background-color: #0d1117;
    color: white;
  }

  .aboutList {
    display: flex;
    flex-direction: row;
    padding: 0.25rem;
    background-color: rgba(255, 255, 255, 0.058);
    border-radius: 2rem;
    gap: 0.5rem;
    justify-content: space-evenly;
  }

  .user {
    display: flex;
    flex-direction: row;
    height: 2rem;
    width: 2rem;
  }

  .userImg {
    border-radius: 1rem;
  }

  .spacer {
    height: 5rem;
  }

  .titleText {
    font-size: 7.5rem;
    font-weight: bolder;
    letter-spacing: -0.5rem;
  }

  .mainLayout {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    height: 100%;
  }

  span {
    text-align: center;
  }

  #__nuxt {
    height: 100%;
  }

  body {
    margin: 0;
    height: 100%;
  }

  html {
    height: 100%;
  }


</style>

<script lang="ts">
export default {
    props: ['error'],
};
</script>

<script setup lang="ts">
useSeoMeta({
  title: 'I am a teapot. Are you?',
  ogTitle: 'I am a teapot. Are you?',
  description: 'The high-quality teapot experience.',
  ogDescription: 'The high-quality teapot experience.',
  ogImage: 'https://http.cat/418',
})
</script>