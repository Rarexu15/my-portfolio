<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
</script>

<template>
    <AppLayout>
        <div class="max-w-3xl mx-auto px-6 py-16">
            <h1 class="text-4xl font-bold text-gray-900 mb-6">About Me</h1>
            <p class="text-gray-700 leading-relaxed mb-4">
                I'm a fourth-year BS Information Technology student at World Citi Colleges,
                Antipolo Campus. I'm motivated, hardworking, and passionate about learning —
                dedicated to delivering quality work and continuously improving my skills.
            </p>
            <p class="text-gray-700 leading-relaxed mb-4">
                I have hands-on experience as a freelance fullstack developer, building systems
                with PHP, MySQL, HTML, and JavaScript, as well as web/database administration
                and graphic design work.
            </p>

            <h2 class="text-2xl font-semibold text-gray-900 mt-10 mb-4">Skills</h2>
            <ul class="grid grid-cols-2 gap-2 text-gray-700 list-disc list-inside">
                <li>Web Development (WordPress, PHP)</li>
                <li>UI/UX & Front-End Design</li>
                <li>Database Management (MySQL)</li>
                <li>JavaScript Basics</li>
                <li>Basic Computer Networking</li>
                <li>Visual Basic Programming</li>
            </ul>

            <h2 class="text-2xl font-semibold text-gray-900 mt-10 mb-4">Experience</h2>
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