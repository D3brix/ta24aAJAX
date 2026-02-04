<script setup>
import { ref } from 'vue';
import Tabs from './components/Tabs.vue';

let titles = ref([
    'item 1',
    'item 2',
    'item 3',
    'item 4',
]);

let activeTab = ref(0);
</script>

<template> 
  <Tabs :titles="titles" :active="activeTab"></Tabs>
    <div class="container">
     
    </div>
</template>

<style></style>