<script>
import Nav from "./Nav.vue";

export default {
    components: {
        Nav
    }
}
</script>

<template>
    <section class="p-6 bg-gray-200">
        <header class="container mx-auto flex items-center justify-between">
            <div class="flex items-end divide-x divide-black">
                <h1 class="font-bold text-lg pr-4">My App</h1>

                <p class="text-sm pl-4">Welcome back, {{ $page.props.auth.user }}!</p>
            </div>

            <Nav />
        </header>
    </section>

    <section class="p-6">
        <div class="container mx-auto">
            <slot />
        </div>
    </section>
</template>
