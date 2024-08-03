<script setup>
import Title from './Title.vue';
import QuestionBox from './QuestionBox.vue';

/**
 * https://www.pbs.org/wgbh/americanexperience/films/houdini/
 * https://www.oldest.org/entertainment/magic-tricks/
 * https://www.finchmagician.com/magic/list-of-magic-tricks
 * https://dennymagic.com/why-do-magicians-use-rabbits/
 *
 * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input/radio#using_radio_inputs
 * https://search.brave.com/search?q=How+to+make+a+multiple+choice+questions+with+js+composition+api+vue
 */
</script>

<template>
    <Title #titleText>
        Trivia
    </Title>

    <div>
        <p class="font-serif text-base text-center py-5">Answer the questions below and select the right answer.</p>
    </div>

    <div id="trivia" class="grid grid-cols-2 gap-8 px-5">
        <QuestionBox>
            <template #question>
                Who was Houdini?
            </template>

            <template #answer1>
                A cow
            </template>

            <template #answer2>
                A magician
            </template>

            <template #answer3>
                A humanoid owl
            </template>

            <template #answer4>
                A storefront's pet name
            </template>
        </QuestionBox>

        <QuestionBox>
            <template #question>
                When was the first magic trick performed?
            </template>

            <template #answer1>
                1589 CE
            </template>

            <template #answer2>
                916 - 925 CE
            </template>

            <template #answer3>
                2700 - 3000 BCE
            </template>

            <template #answer4>
                3200 - 3500 BCE
            </template>
        </QuestionBox>

        <QuestionBox>
            <template #question>
                Which one of the following is a magic trick?
            </template>

            <template #answer1>
                Crazy Man’s Handcuffs
            </template>

            <template #answer2>
                Magician's Illusion
            </template>

            <template #answer3>
                The Notebook Test
            </template>

            <template #answer4>
                Slight of Phantom Hands
            </template>
        </QuestionBox>

        <QuestionBox>
            <template #question>
                Why do magicians like to perform magic tricks with rabbits?
            </template>

            <template #answer1>
                Rabbits like magicians too
            </template>

            <template #answer2>
                Eat carrots
            </template>

            <template #answer3>
                Have space-bending properties
            </template>

            <template #answer4>
                Rabbits are easy to train
            </template>
        </QuestionBox>
    </div>
</template>
