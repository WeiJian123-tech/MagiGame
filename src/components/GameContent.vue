<script setup>
import Title from './Title.vue'
import GameHats from './GameHats.vue'

/*
 * Special thanks to these sources which helped me build this game:
 *
 * This StackOverflow answer by mrrrk(https://stackoverflow.com/users/155791/mrrrk):
 * https://stackoverflow.com/a/61403621
 * asked by user3348410(https://stackoverflow.com/users/3348410/user3348410):
 * https://stackoverflow.com/q/53737648
 *
 * Brave AI for how to make an image clickable: https://search.brave.com/search?q=How+to+make+an+image+clickable+vue
 *
 * Mozilla JavaScript Documentation for how to generate random numbers: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random
 */

function startGame() {

    const gameContainer = document.getElementById('game');
    gameContainer.setAttribute('class', 'grid grid-cols-4 gap-4');

}
function resetGame() {
    const gameContainer = document.getElementById('game');
    gameContainer.setAttribute('class', 'hidden');

    window.location.reload();
}

</script>

<template>
    <Title #titleText>
        Find Rabbit!
    </Title>

    <div class="flex flex-row justify-center align-middle">
        <button type="button" v-on:click="startGame()" class="bg-green-400 mx-2 p-5 border-2 border-black rounded hover:bg-green-300">
            Start Game
        </button>

        <button type="button" v-on:click="resetGame()" class="bg-slate-400 mx-2 p-5 border-2 border-black rounded hover:bg-slate-300">
            Reset/Reload
        </button>
    </div>

    <div>
        <p class="font-serif text-base text-center py-5">
            Find a rabbit to win this game. Click on each top hat to see if a rabbit is hidden underneath it. You have a 5% chance of finding a rabbit. Good luck!
        </p>
    </div>

    <div id="game" class="hidden">
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
        <GameHats />
    </div>

</template>
