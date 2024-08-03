<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>

    <nav class="flex flex-row justify-start bg-cyan-200 text-3xl">
      <div>
        <img alt="Vue logo" class="logo" src="./assets/top_hat_with_rabbit.png" width="32" height="32" />
      </div>
      <div>
        <RouterLink to="/" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Home</RouterLink>
        <RouterLink to="game" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Game</RouterLink>
        <RouterLink to="trivia" class="text-slate-800 hover:text-neutral-950 hover:underline mx-5">Trivia</RouterLink>
      </div>
    </nav>
  </header>

  <RouterView />

</template>
