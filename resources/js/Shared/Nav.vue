<script setup>
import NavLink from "@/Shared/NavLink.vue";
</script>

<template>
    <nav class="p-4">
        <ul class="flex gap-4">
            <li>
                <NavLink href="/" :active="$page.component === 'Home'">
                    Home
                </NavLink>
            </li>
            <li>
                <NavLink href="/users" :active="$page.component === 'Users'">
                    Users
                </NavLink>
            </li>
            <li>
                <NavLink href="/settings" :active="$page.component === 'Settings'">
                    Settings
                </NavLink>
            </li>
        </ul>
    </nav>
</template>
