<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>

    <nav class="flex flex-row justify-start bg-cyan-200 text-3xl">
      <div>
        <!--Placeholder Image-->
        <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="50" height="50" />
      </div>
      <div>
        <RouterLink to="/" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Home</RouterLink>
        <RouterLink to="game" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Game</RouterLink>
        <RouterLink to="trivia" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Trivia</RouterLink>
      </div>
    </nav>
  </header>

  <RouterView />

<!--
  <nav class="flex flex-row justify-start bg-cyan-200 text-3xl">
    <a href="/" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Home</a>
    <a href="/game" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Game</a>
    <a href="/trivia" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Trivia</a>
  </nav>

  <div>
    <h1 class="font-bold text-6xl text-center text-slate-200 py-5">Welcome to MagiGame!</h1>
    <div>
      <img src="./assets/magician.jpg" alt="A magician in a restaurant with a wand pointing his free hand to the camera." class="w-96 h-auto py-1 m-auto">

      <p class="w-full h-auto bg-black text-center">
        Photo by
        <a href="https://unsplash.com/@kouchpeydeh?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash" class="hover:bg-neutral-300/75">
          Khashayar Kouchpeydeh
        </a> on <a href="https://unsplash.com/photos/man-in-black-jacket-playing-guitar-5yVmZ-OqhF4?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash" class="hover:bg-neutral-300/75">
          Unsplash
        </a>
      </p>

    </div>
    <p class="text-wrap text-center align-middle break-words pt-2">
      Come one! Come all! Gather around to this little yet <span class="italic">enchanting</span> website for magician enthusiasts.
      Play a hidden object game! Wrinkle your brain with a small magician trivia. May you feel a bit of magic coursing through your hands with each click!
    </p>
  </div>
-->
</template>

<!--
<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
-->
