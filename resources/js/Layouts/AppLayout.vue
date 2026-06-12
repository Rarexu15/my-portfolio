<script setup>
import { Link, usePage } from '@inertiajs/vue3';

const page = usePage();

const links = [
    { name: 'Home', href: '/' },
    { name: 'About', href: '/about' },
    { name: 'Projects', href: '/projects' },
    { name: 'Contact', href: '/contact' },
];
</script>

<template>
    <div class="min-h-screen bg-gradient-to-b from-indigo-50 via-white to-white flex flex-col">
        <header class="bg-white shadow-sm sticky top-0 z-10">
            <nav class="max-w-4xl mx-auto flex justify-center gap-8 py-5">
                <Link
                    v-for="link in links"
                    :key="link.href"
                    :href="link.href"
                    class="font-medium transition-colors"
                    :class="page.url === link.href
                        ? 'text-indigo-600'
                        : 'text-gray-500 hover:text-indigo-600'"
                >
                    {{ link.name }}
                </Link>
            </nav>
        </header>

        <main class="flex-1">
            <slot />
        </main>

        <footer class="text-center text-sm text-gray-400 py-6">
            © {{ new Date().getFullYear() }} Ralex Anzano. Built with Laravel & Vue.
        </footer>
    </div>
</template>