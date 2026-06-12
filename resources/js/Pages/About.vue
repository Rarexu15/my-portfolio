<script setup>
import { Link } from '@inertiajs/vue3';
</script>

<template>
    <div class="min-h-screen bg-gray-50 flex flex-col">
        <nav class="flex justify-center gap-8 py-6 bg-white shadow-sm">
            <Link href="/" class="text-gray-600 hover:text-gray-900">Home</Link>
            <Link href="/about" class="font-semibold text-gray-800">About</Link>
            <Link href="/projects" class="text-gray-600 hover:text-gray-900">Projects</Link>
            <Link href="/contact" class="text-gray-600 hover:text-gray-900">Contact</Link>
        </nav>

        <main class="flex-1 max-w-3xl mx-auto px-6 py-16">
            <h1 class="text-4xl font-bold text-gray-900 mb-6">About Me</h1>
            <p class="text-gray-700 leading-relaxed mb-4">
                Write a few paragraphs about yourself here — your background, what you're studying,
                and what motivates you to learn web development.
            </p>
            <p class="text-gray-700 leading-relaxed">
                You can also mention your goals, interests outside coding, or fun facts.
            </p>
        </main>
    </div>
</template>