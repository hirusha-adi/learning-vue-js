<script setup>
import { defineProps } from 'vue';

// the names must match
const { quiz } = defineProps(['quiz'])

</script>

<template>
    <div class="card">
        <img :src="quiz.img" :alt="quiz.name">
        <div class="card-text">
            <h2>{{ quiz.name }}</h2>
            <p>{{ quiz.questions.length }} questions</p>
        </div>
    </div>
</template>

<style scoped>
.card {
    width: 310px;
    overflow: hidden;
    border-radius: 2%;
    box-shadow: 5px 5px 20px rbga(0, 0, 0, 0.9);
    margin-bottom: 25px;
    margin-right: 20px;
    cursor: pointer;
}

.card img {
    width: 100%;
    height: 190px;
    margin: 0;
}

.card .card-text {
    padding: 0 5px;
}

.card .card-text h2 {
    font-weight: bold;
}
</style>