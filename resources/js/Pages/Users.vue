<script setup>
defineProps({
    time: String,
    users: Array
})
</script>

<template>
    <Head title="Users" />

    <h1 class="text-2xl font-bold">Users</h1>

    <ul>
        <li
            v-for="user in users"
            :key="user.id"
            v-text="user.name"
        />
    </ul>

    <div class="mt-[1700px] p-10 flex flex-col gap-4">
        <p>Current time is {{ time }}.</p>

        <Link href="/users" preserve-scroll>Refresh</Link>
    </div>
</template>
