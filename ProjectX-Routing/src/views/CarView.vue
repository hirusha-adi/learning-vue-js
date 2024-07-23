<script setup>
import { useRoute } from 'vue-router';
import cars from "../data/cars.json"

const route = useRoute()
// route.params: dict[str, str]

// id is the name of the paramater given the router/index.js
const car = cars.find(c => c.id === parseInt(route.params.id))

</script>

<template>
    <h1>car view</h1>
    <br>
    <hr>
    <p>{{ car.name }}</p>
    <p>{{ car.price }}</p>
    <p>{{ car.year }}</p>
</template>