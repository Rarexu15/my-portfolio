<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
</script>

<template>
    <AppLayout>
        <div class="max-w-6xl mx-auto px-6 py-16 grid md:grid-cols-2 gap-12 items-center">
            <div>
                <p class="text-primary font-semibold tracking-wide mb-2 text-sm uppercase">
                    BSIT Student / Fullstack Developer
                </p>
                <h1 class="text-5xl font-bold text-gray-900 mb-4 leading-tight">
                    Hello, my name is Ralex Anzano
                </h1>
                <p class="text-gray-600 mb-6 max-w-md">
                    A 4th-year BS Information Technology student passionate about web
                    development, UI/UX, and building practical solutions.
                </p>
                <div class="flex gap-3">
                    <a href="/projects" class="bg-primary text-white px-6 py-2.5 rounded-lg font-medium hover:bg-primary/80 transition-colors">
                        Projects
                    </a>
                    <a href="https://github.com/Rarexu15" target="_blank" class="border border-gray-300 px-6 py-2.5 rounded-lg font-medium hover:bg-gray-50 transition-colors">
                        GitHub
                    </a>
                </div>
            </div>

            <div class="relative flex justify-center">
                <div class="absolute w-72 h-72 bg-sage rounded-[40%_60%_60%_40%/60%_40%_60%_40%]"></div>
                <img
                    src="/images/profile.jpg"
                    alt="Ralex Anzano"
                    class="relative w-64 h-64 rounded-full object-cover shadow-lg z-10"
                />
            </div>
        </div>
    </AppLayout>
</template>