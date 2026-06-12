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
    <div class="min-h-screen bg-cream flex flex-col">
        <header class="bg-white shadow-sm sticky top-0 z-100">
            <nav class="max-w-5xl mx-auto flex items-center justify-between px-6 py-5">
                <span class="font-bold text-gray-900">Ralex Anzano</span>
                <div class="flex gap-8">
                    <Link
                        v-for="link in links"
                        :key="link.href"
                        :href="link.href"
                        class="font-medium transition-colors"
                        :class="page.url === link.href
                            ? 'text-primary'
                            : 'text-gray-500 hover:text-primary'"
                    >
                        {{ link.name }}
                    </Link>
                </div>
            </nav>
        </header>

        <main class="flex-1">
            <slot />
        </main>

        <footer class="text-center text-sm text-gray-500 py-6">
            © {{ new Date().getFullYear() }} Ralex Anzano. Built with Laravel & Vue.
        </footer>
    </div>
</template>