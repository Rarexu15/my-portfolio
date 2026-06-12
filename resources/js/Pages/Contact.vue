<script setup>
import AppLayout from '@/Layouts/AppLayout.vue';
import { useForm, usePage } from '@inertiajs/vue3';

const page = usePage();

const form = useForm({
    name: '',
    email: '',
    message: '',
});

const submit = () => {
    form.post('/contact', {
        onSuccess: () => form.reset(),
    });
};
</script>

<template>
    <AppLayout>
        <div class="max-w-2xl mx-auto px-6 py-16">
            <h1 class="text-4xl font-bold text-gray-900 mb-2">Contact</h1>
            <div class="w-16 h-1 bg-primary mb-10 rounded"></div>

            <div v-if="page.props.flash?.success"
                 class="mb-6 p-4 bg-sage/30 border border-sage text-gray-800 rounded-lg">
                {{ page.props.flash.success }}
            </div>

            <form @submit.prevent="submit" class="space-y-5 bg-white p-8 rounded-2xl shadow">
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Name</label>
                    <input v-model="form.name" type="text"
                           class="w-full border border-gray-300 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-secondary" />
                    <p v-if="form.errors.name" class="text-red-500 text-sm mt-1">{{ form.errors.name }}</p>
                </div>
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Email</label>
                    <input v-model="form.email" type="email"
                           class="w-full border border-gray-300 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-secondary" />
                    <p v-if="form.errors.email" class="text-red-500 text-sm mt-1">{{ form.errors.email }}</p>
                </div>
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Message</label>
                    <textarea v-model="form.message" rows="5"
                              class="w-full border border-gray-300 rounded-lg px-4 py-2 focus:outline-none focus:ring-2 focus:ring-secondary"></textarea>
                    <p v-if="form.errors.message" class="text-red-500 text-sm mt-1">{{ form.errors.message }}</p>
                </div>
                <button type="submit" :disabled="form.processing"
                        class="bg-primary text-white px-6 py-2.5 rounded-lg font-medium hover:bg-primary/80 transition-colors disabled:opacity-50">
                    {{ form.processing ? 'Sending...' : 'Send' }}
                </button>
            </form>

            <div class="mt-8 text-center text-gray-700 space-y-2">
                <p>Email: <a href="mailto:anzanoralex@gmail.com" class="text-primary hover:underline">anzanoralex@gmail.com</a></p>
                <p>Phone: 0951 447 3219</p>
                <p>GitHub: <a href="https://github.com/Rarexu15" target="_blank" class="text-primary hover:underline">github.com/Rarexu15</a></p>
            </div>
        </div>
    </AppLayout>
</template>