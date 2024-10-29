<script setup>
import Layout from '@/Shared/Layout.vue';
import {Link} from "@inertiajs/vue3";

defineProps({
    time: String,
})
</script>

<template>
    <Layout>
        <h1 class="text-2xl font-bold">Users</h1>

        <div class="mt-[1700px] p-10 flex flex-col gap-4">
            <p>Current time is {{ time }}.</p>

            <Link href="/users" preserve-scroll>Refresh</Link>
        </div>
    </Layout>
</template>
