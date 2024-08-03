<script setup>
import topHat from '../assets/magician_top_hat.png'
import rabbit from '../assets/top_hat_with_rabbit.png'
import liftedTopHat from '../assets/lifted_top_hat.png'
import { ref, onMounted } from 'vue'

let hat = ref(topHat);

//When the player clicks a top hat image, generate a random chance for Rabbit to appear to replace top hat. Else replace with LiftedTopHat.
async function revealHat(event) {

    const randomRabbitPull = Math.floor(Math.random() * 100);
    console.log(randomRabbitPull);

    const hatTarget = event.target;
    console.log(hatTarget);
    console.log(hatTarget.src);


    if(randomRabbitPull > 45) {
        hat.value = rabbit;
        hatTarget.alt = 'Image of a top hat with a rabbit revealed from underneath it.'
        console.log("hat: " + hat.value);
    } else {
        hat.value = liftedTopHat;
        hatTarget.alt = 'Image of a top hat lifted from its rim to reveal no rabbit.'
        console.log("hat: " + hat.value);
    }

    onMounted(async () => {
        hat.value.click();
    });

}
</script>

<template>
    <div>
        <button type="button" @click="revealHat($event)">
            <img :src="hat" alt="Image of a magician top hat" class="hover:max-w-[110%]"/>
        </button>
    </div>
</template>
