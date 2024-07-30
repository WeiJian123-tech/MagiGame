<script setup>
import Title from './Title.vue'
import topHat from '../assets/magician_top_hat.png'
import liftedTopHat from '../assets/lifted_top_hat.png'
import rabbit from '../assets/top_hat_with_rabbit.png'

function startGame() {

    const hiddenRabbit = document.createElement('img');
    hiddenRabbit.src = rabbit;
    hiddenRabbit.alt = 'A rabbit revealed hidden under a top hat';

    const rabbitLocation = Math.floor(Math.random() * 16) + 1;
    console.log(rabbitLocation);

    let topHatLocation = document.getElementById(rabbitLocation);

    topHatLocation.replaceChild(hiddenRabbit, topHatLocation.firstChild); //May replace images with buttons

    //https://search.brave.com/search?q=How+to+make+an+image+clickable+vue
}

function resetGame() {

}

</script>

<template>
    <Title #titleText>
        Find the Rabbit!
    </Title>

    <div class="flex flex-row justify-center align-middle">
        <button type="button" v-on:click="startGame()" class="bg-green-400 mx-2 p-5 border-2 border-black rounded hover:bg-green-300">
            Start Game
        </button>

        <button type="button" v-on:click="resetGame()" class="bg-slate-400 mx-2 p-5 border-2 border-black rounded hover:bg-slate-300">
            Reset
        </button>
    </div>

    <div id="game" class="grid grid-cols-4 gap-4">
        <div class="imgCont" id="1">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="2">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="3">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="4">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="5">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="6">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="7">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="8">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="9">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="10">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="11">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="12">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="13">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="14">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="15">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
        <div class="imgCont" id="16">
            <img :src="topHat" alt="Image of a magician top hat" class="hover:cursor-pointer hover:max-w-[110%]"/>
        </div>
    </div>

</template>
