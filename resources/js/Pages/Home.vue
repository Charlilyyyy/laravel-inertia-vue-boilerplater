<script setup>
import { useForm } from '@inertiajs/vue3'
import TextInput from '@Components/TextInput.vue'
import Dropdown from '@Components/Dropdown.vue';

const form = useForm({
    email: null,
    password: null,
    remember: null,
    dropdown: null, // Added this for dropdown binding
});

const items = ['key','fork','spoon']
</script>

<template>
    home vue , laravel , inertia , tailwind
    <div>
        <p class="text-slate-500">
            I’m Derek, an astro-engineer based in Tattooine. I like to build X-Wings at
            <a class="underline decoration-sky-500/30">My Company, Inc</a>.
            Outside of work, I like to <a class="underline decoration-pink-500/30">watch
            pod-racing</a> and have <a class="underline decoration-indigo-500/30">light-saber</a> fights.
        </p>
    </div>

    <div>
        <TextInput
            labelName="Email"
            type="email"
            v-model="form.email"
            :message="form.errors.email"
        />
        <TextInput
            labelName="Email"
            type="email"
            v-model="form.email"
            :message="form.errors.email"
        />
    </div>
    <div>
        <Dropdown
            labelName="Select an Item"
            name="Please select"
            :items="items"
            v-model="form.dropdown"
            :message="form.errors.dropdown"
        />
    </div>
</template>
