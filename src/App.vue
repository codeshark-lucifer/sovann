<script setup lang="ts">
import Navigation from './components/Navigation.vue';

</script>

<template>
    <header>
        <Navigation/>
    </header>
    <main>
        <RouterView/>
    </main>
</template>