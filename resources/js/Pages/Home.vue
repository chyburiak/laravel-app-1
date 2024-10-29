<script setup>
    import Nav from '@/Shared/Nav.vue';
    import {Link} from "@inertiajs/vue3";

    defineProps({
        time: String,
    })
</script>

<template>
    <Nav />

    <h1>Home</h1>

    <div class="mt-[1700px] p-10 flex flex-col gap-4">
        <p>Current time is {{ time }}.</p>

        <Link href="/" preserve-scroll>Refresh</Link>
    </div>
</template>
