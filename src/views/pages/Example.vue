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
        <!-- 1st row -->
        <div class="col-span-12 xl:col-span-12">
            <div class="card mb-0 h-40">

            </div>
        </div>

        <!-- 2nd rows -->
        <div class="col-span-12 xl:col-span-4 lg:col-span-6">
            <div class="card mb-0 h-32"></div>
        </div>
        <div class="col-span-12 xl:col-span-4 lg:col-span-6">
            <div class="card mb-0 h-32"></div>
        </div>
        <div class="col-span-12 xl:col-span-4 lg:col-span-6">
            <div class="card mb-0 h-32"></div>
        </div>
        
        <!-- 3rd rows -->
        <div class="col-span-12 xl:col-span-6">
            <div class="card mb-0 h-80"></div>
        </div>

        <div class="col-span-12 xl:col-span-6">
            <div class="card mb-0 h-80"></div>
        </div>

        <!-- 4th rows -->
        <div class="col-span-12">
            <div class="card mb-0 h-96"></div>
        </div> 
    </div>
</template>
