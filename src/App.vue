<script setup>
import { ref } from 'vue';
import Modal from './components/Modal.vue';

let modalActive = ref(false)

let value = modalActive ? 'modal is-active' : 'modal';
</script>

<template>
    <div class="container">
        <button class="button is-primary" @click="modalActive = true">Open Modal</button>
        <Modal :active="modalActive" @close="modalActive=false"></Modal>
        
    </div>
</template>

<style></style>