<script setup>
import cars from "../data/cars.json"
import { RouterLink } from "vue-router";
</script>

<template>
    <h1>home view</h1>
    <br>
    <hr>
    <div>
        <ul>
            <li v-for="car in cars" :key="car.id">
                <RouterLink :to="`/car/${car.id}`">
                    {{ car.name }}
                </RouterLink>
            </li>
        </ul>
    </div>
</template>