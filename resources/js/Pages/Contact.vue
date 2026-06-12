<script setup>
import { Link } from '@inertiajs/vue3';
</script>

<template>
    <div class="min-h-screen bg-gray-50 flex flex-col">
        <nav class="flex justify-center gap-8 py-6 bg-white shadow-sm">
            <Link href="/" class="text-gray-600 hover:text-gray-900">Home</Link>
            <Link href="/about" class="text-gray-600 hover:text-gray-900">About</Link>
            <Link href="/projects" class="text-gray-600 hover:text-gray-900">Projects</Link>
            <Link href="/contact" class="font-semibold text-gray-800">Contact</Link>
        </nav>

        <main class="flex-1 max-w-2xl mx-auto px-6 py-16 text-center">
            <h1 class="text-4xl font-bold text-gray-900 mb-6">Get In Touch</h1>
            <p class="text-gray-700 mb-8">
                Feel free to reach out through any of these channels:
            </p>
            <div class="space-y-3">
                <p class="text-gray-800">
                    Email:
                    <a href="mailto:youremail@example.com" class="text-blue-600 hover:underline">
                        youremail@example.com
                    </a>
                </p>
                <p class="text-gray-800">
                    GitHub:
                    <a href="https://github.com/Rarexu15" target="_blank" class="text-blue-600 hover:underline">
                        github.com/Rarexu15
                    </a>
                </p>
                <p class="text-gray-800">
                    LinkedIn:
                    <a href="#" target="_blank" class="text-blue-600 hover:underline">
                        linkedin.com/in/yourname
                    </a>
                </p>
            </div>
        </main>
    </div>
</template>