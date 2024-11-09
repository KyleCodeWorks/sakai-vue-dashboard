<script setup>
import { ref } from 'vue';

const dropdownValues = ref([
    { name: 'New York', code: 'NY' },
    { name: 'Rome', code: 'RM' },
    { name: 'London', code: 'LDN' },
    { name: 'Istanbul', code: 'IST' },
    { name: 'Paris', code: 'PRS' }
]);
const dropdownValue = ref(null);
</script>
<template>
    <!-- <div class="card">
        <div class="font-semibold text-xl mb-4">My Dashboard</div>
        <div class="flex flex-row md:flex-col mb-4">
            <div class="w-1/4 mb-4 md:mb-0 md:mr-4">
                <InputGroup>
                    <InputGroupAddon> Year </InputGroupAddon>
                    <Select v-model="dropdownValue" :options="dropdownValues" optionLabel="name" placeholder="Select" />
                </InputGroup>
            </div>
        </div>
        <p>Use this page to start from scratch and place your custom content.</p>
    </div> -->
    <div class="grid grid-cols-12 gap-8">
        <div class="col-span-12 lg:col-span-6 xl:col-span-3">
            <div class="card mb-0"></div>
        </div>
        <div class="col-span-12 lg:col-span-6 xl:col-span-3">
            <div class="card mb-0"></div>
        </div>
        <div class="col-span-12 lg:col-span-6 xl:col-span-3">
            <div class="card mb-0"></div>
        </div>
        <div class="col-span-12 lg:col-span-6 xl:col-span-3">
            <div class="card mb-0"></div>
        </div>
    </div>
</template>
