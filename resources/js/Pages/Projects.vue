<script setup>
import { Link } from '@inertiajs/vue3';

const projects = [
    {
        title: 'Capstone Project: MemoryMate Mobile App',
        description: 'A short description of what this project does and what you used to build it.',
        link: 'https://play.google.com/store/apps/details?id=com.app.memorymate',
    },
     {
        title: 'Allowance Management System',
        description: 'A custom system to track and distribute individual allowance records, built with PHP, MySQL, HTML, and JavaScript. Includes secure interfaces for expense logging and summary viewing.',
        link: '#',
    },
    {
        title: 'Antipolo City Police Station Website',
        description: 'A WordPress-based website with database structures for managing station attendance and timekeeping.',
        link: '#',
    },
    {
        title: 'Fuwa Fuwa Plan Branding',
        description: 'Visual assets created for print and digital marketing campaigns, contributing to a 20% increase in brand visibility.',
        link: '#',
    },
];
</script>

<template>
    <div class="min-h-screen bg-gray-50 flex flex-col">
        <nav class="flex justify-center gap-8 py-6 bg-white shadow-sm">
            <Link href="/" class="text-gray-600 hover:text-gray-900">Home</Link>
            <Link href="/about" class="text-gray-600 hover:text-gray-900">About</Link>
            <Link href="/projects" class="font-semibold text-gray-800">Projects</Link>
            <Link href="/contact" class="text-gray-600 hover:text-gray-900">Contact</Link>
        </nav>

        <main class="flex-1 max-w-4xl mx-auto px-6 py-16 w-full">
            <h1 class="text-4xl font-bold text-gray-900 mb-10">My Projects</h1>
            <div class="grid gap-6 md:grid-cols-2">
                <div v-for="project in projects" :key="project.title"
                     class="bg-white rounded-lg shadow p-6">
                    <h2 class="text-xl font-semibold text-gray-900 mb-2">{{ project.title }}</h2>
                    <p class="text-gray-600 mb-4">{{ project.description }}</p>
                    <a :href="project.link" class="text-blue-600 hover:underline">View Project →</a>
                </div>
            </div>
        </main>
    </div>
</template>