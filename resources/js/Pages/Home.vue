<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
</script>

<template>
    <AppLayout>
        <div class="flex flex-col items-center justify-center text-center px-4 py-24">
            <img src="/images/profile.jpg"
                alt="Ralex Anzano"
                class="w-40 h-40 rounded-full object-cover shadow-lg mb-6 border-4 border-white"/>
            <h1 class="text-5xl font-bold text-gray-900 mb-4">Hi, I'm Ralex Anzano</h1>
            <p class="text-xl text-gray-600 max-w-xl mb-8">
                A 4th-year BS Information Technology student and Fullstack Developer,
                passionate about web development, UI/UX, and building practical solutions.
            </p>
            <div class="flex gap-4">
                <a href="/projects" class="bg-indigo-600 text-white px-6 py-3 rounded-lg font-medium hover:bg-indigo-700 transition-colors">
                    View My Work
                </a>
                <a href="/contact" class="border border-indigo-600 text-indigo-600 px-6 py-3 rounded-lg font-medium hover:bg-indigo-50 transition-colors">
                    Contact Me
                </a>
            </div>
        </div>
    </AppLayout>
</template>