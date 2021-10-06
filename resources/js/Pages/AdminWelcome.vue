<template>
    <Head title="Welcome" />

    <BreezeAuthenticatedLayout>
        <template #header>
            <h2 class="font-semibold text-xl text-gray-800 leading-tight">
                Dashboard/Welcome
            </h2>
        </template>

        <Welcome></Welcome>
    </BreezeAuthenticatedLayout>
</template>

<script>
import BreezeAuthenticatedLayout from '@/Layouts/Authenticated.vue'
import { Head } from '@inertiajs/inertia-vue3';
import Welcome from "@/Pages/Welcome";

export default {
    components: {
        Welcome,
        BreezeAuthenticatedLayout,
        Head,
    },
}
</script>
