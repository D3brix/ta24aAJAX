<script setup>
import { ref } from 'vue';

let modalActive = ref(false)

let value = modalActive ? 'modal is-active' : 'modal';
</script>

<template>
    <div class="container">
        <button class="button is-primary" @click="modalActive = true">Open Modal</button>
        <div :class="modalActive ? 'modal is-active' : 'modal'">
            <div class="modal-background" @click="modalActive = false"></div>
            <div class="modal-content">
                <p class="image is-4by3">
                    <img src="https://bulma.io/assets/images/placeholders/1280x960.png" alt="">
                </p>
            </div>
            <button class="modal-close is-large" aria-label="close"></button>
        </div>
    </div>
</template>

<style></style>