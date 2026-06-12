<script setup>
import { Link } from '@inertiajs/vue3';
</script>

<template>
    <div class="min-h-screen bg-gray-50 flex flex-col">
        <nav class="flex justify-center gap-8 py-6 bg-white shadow-sm">
            <Link href="/" class="font-semibold text-gray-800">Home</Link>
            <Link href="/about" class="text-gray-600 hover:text-gray-900">About</Link>
            <Link href="/projects" class="text-gray-600 hover:text-gray-900">Projects</Link>
            <Link href="/contact" class="text-gray-600 hover:text-gray-900">Contact</Link>
        </nav>

        <main class="flex-1 flex flex-col items-center justify-center text-center px-4">
            <h1 class="text-5xl font-bold text-gray-900 mb-4">Hi, I'm Ralex Anzano</h1>
            <p class="text-xl text-gray-600 max-w-xl">
            A 4th-year BS Information Technology student and Fullstack Developer,
            passionate about web development, UI/UX, and building practical solutions.
            </p>
        </main>
    </div>
</template>