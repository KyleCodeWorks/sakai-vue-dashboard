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

    <div class="grid grid-cols-12 gap-4">
        <!-- 1st row -->

        <div class="col-span-12 md:col-span-4 xl:col-span-4">
            <InputGroup>
                <InputGroupAddon> Year </InputGroupAddon>
                <Select v-model="dropdownValue" :options="dropdownValues" optionLabel="name" placeholder="Select City" />
            </InputGroup>
        </div>

        <!-- 2nd rows -->

        <div class="col-span-12"></div>
        <div class="col-span-12 xl:col-span-4 lg:col-span-6">
            <div class="card mb-0 border-2 border-sky-500">
                <div class="flex justify-between mb-4">
                    <div>
                        <span class="block text-muted-color font-medium mb-4">Customers</span>
                        <div class="text-surface-900 dark:text-surface-0 font-medium text-xl">28441</div>
                    </div>
                    <div class="flex items-center justify-center bg-cyan-100 dark:bg-cyan-400/10 rounded-border" style="width: 2.5rem; height: 2.5rem">
                        <i class="pi pi-users text-cyan-500 !text-xl"></i>
                    </div>
                </div>
                <span class="text-primary font-medium">520 </span>
                <span class="text-muted-color">newly registered</span>
            </div>
        </div>
        <div class="col-span-12 xl:col-span-4 lg:col-span-6">
            <div class="card mb-0 border-2 border-sky-500">
                <div class="flex justify-between mb-4">
                    <div>
                        <span class="block text-muted-color font-medium mb-4">Comments</span>
                        <div class="text-surface-900 dark:text-surface-0 font-medium text-xl">152 Unread</div>
                    </div>
                    <div class="flex items-center justify-center bg-purple-100 dark:bg-purple-400/10 rounded-border" style="width: 2.5rem; height: 2.5rem">
                        <i class="pi pi-comment text-purple-500 !text-xl"></i>
                    </div>
                </div>
                <span class="text-primary font-medium">85 </span>
                <span class="text-muted-color">responded</span>
            </div>
        </div>
        <div class="col-span-12 xl:col-span-4 lg:col-span-6">
            <div class="card mb-0 border-2 border-sky-500">
                <div class="flex justify-between mb-4">
                    <div>
                        <span class="block text-muted-color font-medium mb-4">Orders</span>
                        <div class="text-surface-900 dark:text-surface-0 font-medium text-xl">152</div>
                    </div>
                    <div class="flex items-center justify-center bg-blue-100 dark:bg-blue-400/10 rounded-border" style="width: 2.5rem; height: 2.5rem">
                        <i class="pi pi-shopping-cart text-blue-500 !text-xl"></i>
                    </div>
                </div>
                <span class="text-primary font-medium">24 new </span>
                <span class="text-muted-color">since last visit</span>
            </div>
        </div>

        <!-- <div class="col-span-12 xl:col-span-6">
            <div class="card mb-0 h-80 border-2 border-sky-500"></div>
        </div>

        <div class="col-span-12 xl:col-span-6">
            <div class="card mb-0 h-80 border-2 border-sky-500"></div>
        </div>

        <div class="col-span-12">
            <div class="card mb-0 h-96 border-2 border-sky-500"></div>
        </div> -->
    </div>
</template>
