<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';

const projects = [
    {
        title: 'Capstone Project: MemoryMate Mobile App',
        description: 'A mobile app project — add a short description of what it does and the tools used to build it.',
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
    <AppLayout>
        <div class="max-w-4xl mx-auto px-6 py-16">
            <h1 class="text-4xl font-bold text-gray-900 mb-10">My Projects</h1>
            <div class="grid gap-6 md:grid-cols-2">
                <div v-for="project in projects" :key="project.title"
                     class="bg-white rounded-lg shadow hover:shadow-md transition-shadow p-6">
                    <h2 class="text-xl font-semibold text-gray-900 mb-2">{{ project.title }}</h2>
                    <p class="text-gray-600 mb-4">{{ project.description }}</p>
                    <a :href="project.link" target="_blank" class="text-indigo-600 hover:underline">View Project →</a>
                </div>
            </div>
        </div>
    </AppLayout>
</template>