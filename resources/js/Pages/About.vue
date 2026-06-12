<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
</script>

<template>
    <AppLayout>
        <div class="max-w-6xl mx-auto px-6 py-16 grid md:grid-cols-2 gap-12 items-center mb-16">
            <div>
                <h1 class="text-4xl font-bold text-gray-900 mb-6">About me</h1>
                <p class="text-gray-700 leading-relaxed mb-4">
                    I'm a fourth-year BS Information Technology student at World Citi Colleges,
                    Antipolo Campus. I'm motivated, hardworking, and passionate about learning —
                    dedicated to delivering quality work and continuously improving my skills.
                </p>
                <p class="text-gray-700 leading-relaxed mb-6">
                    I have hands-on experience as a freelance fullstack developer, building
                    systems with PHP, MySQL, HTML, and JavaScript, as well as web/database
                    administration and graphic design work.
                </p>
                <a href="/contact" class="inline-block bg-primary text-white px-6 py-2.5 rounded-lg font-medium hover:bg-primary/80 transition-colors">
                    Contact Me
                </a>
            </div>

            <div class="relative flex justify-center">
                <div class="absolute w-72 h-72 bg-blush rounded-[60%_40%_40%_60%/40%_60%_40%_60%]"></div>
                <img
                    src="/images/profile.jpg"
                    alt="Ralex Anzano"
                    class="relative w-64 h-64 rounded-full object-cover shadow-lg z-10"
                />
            </div>
        </div>

        <div class="max-w-4xl mx-auto px-6 pb-16">
            <h2 class="text-2xl font-semibold text-gray-900 mb-4">Skills</h2>
            <ul class="grid grid-cols-2 gap-2 text-gray-700 list-disc list-inside mb-10">
                <li>Web Development (WordPress, PHP)</li>
                <li>UI/UX & Front-End Design</li>
                <li>Database Management (MySQL)</li>
                <li>JavaScript Basics</li>
                <li>Basic Computer Networking</li>
                <li>Visual Basic Programming</li>
            </ul>

            <h2 class="text-2xl font-semibold text-gray-900 mb-4">Experience</h2>
            <div class="space-y-4 text-gray-700">
                <div>
                    <p class="font-semibold">Freelance Fullstack Developer (June 2025 – December 2025)</p>
                    <p>Developed a custom Allowance Management System using PHP, MySQL, HTML, and JavaScript.</p>
                </div>
                <div>
                    <p class="font-semibold">Web & Database Administrator — Antipolo City Police Station (Oct–Dec 2023)</p>
                    <p>Built a WordPress website and maintained database structures for attendance and timekeeping.</p>
                </div>
                <div>
                    <p class="font-semibold">Graphic Designer — Fuwa Fuwa Plan (Oct 2021 – Dec 2022)</p>
                    <p>Created visual assets for print and digital marketing campaigns, contributing to a 20% increase in brand visibility.</p>
                </div>
            </div>
        </div>
    </AppLayout>
</template>