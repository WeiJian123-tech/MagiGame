<script setup>
import Title from './Title.vue'
</script>

<template>
    <Title #titleText>
        Welcome to MagiGame!
    </Title>

    <div>
      <img src="/src/assets/magician.jpg" alt="A magician in a restaurant with a wand pointing his free hand to the camera." class="w-96 h-auto py-1 m-auto">

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

</template>
