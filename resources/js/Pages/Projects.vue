<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';

const projects = [
    {
        title: 'Capstone Project: MemoryMate Mobile App',
        description: 'A mobile app project — add a short description of what it does and the tools used to build it.',
        link: 'https://play.google.com/store/apps/details?id=com.app.memorymate',
        image: '/images/projects/mm.jpg',
    },
    {
        title: 'Allowance Management System',
        description: 'A custom system to track and distribute individual allowance records, built with PHP, MySQL, HTML, and JavaScript. Includes secure interfaces for expense logging and summary viewing.',
        link: '#',
        image: '/images/projects/allowance.jpg',
    },
    {
        title: 'Antipolo City Police Station Website',
        description: 'A WordPress-based website with database structures for managing station attendance and timekeeping.',
        link: '#',
        image: '/images/projects/police-station.jpg',
    },
    {
        title: 'Fuwa Fuwa Plan Branding',
        description: 'Visual assets created for print and digital marketing campaigns, contributing to a 20% increase in brand visibility.',
        link: '#',
        image: '/images/projects/fuwafuwa.jpg',
    },
];
</script>

<template>
    <AppLayout>
        <div class="max-w-5xl mx-auto px-6 py-16">
            <h1 class="text-4xl font-bold text-gray-900 mb-2">Projects</h1>
            <div class="w-16 h-1 bg-primary mb-12 rounded"></div>

            <div class="space-y-8">
                <div
                    v-for="(project, index) in projects"
                    :key="project.title"
                    class="bg-white rounded-2xl shadow overflow-hidden grid md:grid-cols-2"
                    :class="index % 2 === 1 ? 'md:[&>div:first-child]:order-2' : ''"
                >
                    <div class="p-8 flex flex-col justify-center">
                        <h2 class="text-2xl font-semibold text-gray-900 mb-3">{{ project.title }}</h2>
                        <p class="text-gray-600 mb-5">{{ project.description }}</p>
                        <a :href="project.link" target="_blank"
                           class="inline-block border border-primary text-primary px-5 py-2 rounded-lg font-medium hover:bg-primary hover:text-white transition-colors w-fit">
                            View Project
                        </a>
                    </div>
                    <div class="bg-cream min-h-[250px]"
                         :style="{ backgroundImage: `url(${project.image})`, backgroundSize: 'cover', backgroundPosition: 'center' }">
                    </div>
                </div>
            </div>
        </div>
    </AppLayout>
</template>