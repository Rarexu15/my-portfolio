<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
</script>

<template>
    <AppLayout>
        <!-- Header band -->
        <div class="bg-blush">
            <div class="max-w-4xl mx-auto px-6 py-12 flex flex-col md:flex-row items-center gap-6">
                <img
                    src="/images/profile.jpg"
                    alt="Ralex Anzano"
                    class="w-32 h-32 rounded-full object-cover shadow-lg border-4 border-white"
                />
                <div class="text-center md:text-left">
                    <h1 class="text-3xl font-bold text-gray-900">Ralex Anzano</h1>
                    <p class="text-primary font-medium">BSIT Student / Fullstack Developer</p>
                    <p class="text-gray-600 text-sm mt-1">Antipolo, Rizal, Philippines</p>
                </div>
            </div>
        </div>

        <div class="max-w-4xl mx-auto px-6 py-12 space-y-12">
            <!-- About -->
            <section>
                <h2 class="text-xl font-bold text-gray-900 mb-3 pb-2 border-b-2 border-primary inline-block">About</h2>
                <p class="text-gray-700 leading-relaxed mb-3">
                    I'm a fourth-year BS Information Technology student at World Citi Colleges,
                    Antipolo Campus. I'm motivated, hardworking, and passionate about learning —
                    dedicated to delivering quality work and continuously improving my skills.
                </p>
                <p class="text-gray-700 leading-relaxed">
                    I have hands-on experience as a freelance fullstack developer, building
                    systems with PHP, MySQL, HTML, and JavaScript, as well as web/database
                    administration and graphic design work.
                </p>
            </section>

            <!-- Skills -->
            <section>
                <h2 class="text-xl font-bold text-gray-900 mb-3 pb-2 border-b-2 border-primary inline-block">Skills</h2>
                <div class="flex flex-wrap gap-2">
                    <span v-for="skill in [
                        'Web Development (WordPress, PHP)',
                        'UI/UX & Front-End Design',
                        'Database Management (MySQL)',
                        'JavaScript Basics',
                        'Basic Computer Networking',
                        'Visual Basic Programming',
                    ]" :key="skill"
                    class="bg-cream text-gray-800 text-sm px-3 py-1.5 rounded-full">
                        {{ skill }}
                    </span>
                </div>
            </section>

            <!-- Experience -->
            <section>
                <h2 class="text-xl font-bold text-gray-900 mb-4 pb-2 border-b-2 border-primary inline-block">Experience</h2>
                <div class="space-y-6">
                    <div class="flex gap-4">
                        <div class="w-1 bg-primary rounded-full"></div>
                        <div>
                            <p class="font-semibold text-gray-900">Freelance Fullstack Developer</p>
                            <p class="text-sm text-gray-500 mb-1">June 2025 – December 2025</p>
                            <p class="text-gray-700">Developed a custom Allowance Management System using PHP, MySQL, HTML, and JavaScript.</p>
                        </div>
                    </div>
                    <div class="flex gap-4">
                        <div class="w-1 bg-primary rounded-full"></div>
                        <div>
                            <p class="font-semibold text-gray-900">Web & Database Administrator — Antipolo City Police Station</p>
                            <p class="text-sm text-gray-500 mb-1">October 2023 – December 2023</p>
                            <p class="text-gray-700">Built a WordPress website and maintained database structures for attendance and timekeeping.</p>
                        </div>
                    </div>
                    <div class="flex gap-4">
                        <div class="w-1 bg-primary rounded-full"></div>
                        <div>
                            <p class="font-semibold text-gray-900">Graphic Designer — Fuwa Fuwa Plan</p>
                            <p class="text-sm text-gray-500 mb-1">October 2021 – December 2022</p>
                            <p class="text-gray-700">Created visual assets for print and digital marketing campaigns, contributing to a 20% increase in brand visibility.</p>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Education -->
            <section>
                <h2 class="text-xl font-bold text-gray-900 mb-4 pb-2 border-b-2 border-primary inline-block">Education</h2>
                <div class="space-y-4">
                    <div>
                        <p class="font-semibold text-gray-900">World Citi Colleges, Antipolo Campus</p>
                        <p class="text-gray-700">Bachelor of Science in Information Technology</p>
                        <p class="text-sm text-gray-500">2022 – Present</p>
                    </div>
                    <div>
                        <p class="font-semibold text-gray-900">Morong National High School</p>
                        <p class="text-gray-700">Science, Technology, Engineering and Mathematics</p>
                        <p class="text-sm text-gray-500">2020 – 2022</p>
                    </div>
                </div>
            </section>

            <div class="text-center pt-4">
                <a href="/contact" class="inline-block bg-primary text-white px-6 py-2.5 rounded-lg font-medium hover:bg-primary/80 transition-colors">
                    Contact Me
                </a>
            </div>
        </div>
    </AppLayout>
</template>