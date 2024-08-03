<script setup>
</script>

<template>
    <div class="bg-slate-300">
        <form>
            <fieldset>
                <legend>
                    <slot name="question"></slot>
                </legend>

                <div class=" bg-slate-400">
                    <div>
                        <input type="radio" id="choice1" name="choice" checked />
                        <label for="choice1">
                            <slot name="answer1"></slot>
                        </label>
                    </div>

                    <div>
                        <input type="radio" id="choice2" name="choice" />
                        <label for="choice2">
                            <slot name="answer2"></slot>
                        </label>
                    </div>

                    <div>
                        <input type="radio" id="choice3" name="choice" />
                        <label for="choice3">
                            <slot name="answer3"></slot>
                        </label>
                    </div>

                    <div>
                        <input type="radio" id="choice4" name="choice" />
                        <label for="choice4">
                            <slot name="answer4"></slot>
                        </label>
                    </div>

                </div>

                <div>
                    <button type="submit" class="bg-white p-2 hover:bg-slate-100">SUBMIT</button>
                </div>
            </fieldset>
        </form>
    </div>
</template>
