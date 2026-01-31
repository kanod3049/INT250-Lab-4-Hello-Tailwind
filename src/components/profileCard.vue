<script setup>
    defineProps([
        "profileimg",
        "background",
        "name",
        "subheading",
        "followers",
        "following",
        "projects"
    ]);
</script>

<template>
    <div class="bg-white shadow-lg rounded-2xl min-[320px] overflow-hidden text-center">
        <div class="relative min-h-32 bg-cover bg-center" :style="'background-image: url(' + background +')'">
            <img :src="profileimg" alt="Profile Images" class="inline-block w-32 h-32 rounded-full object-center object-cover border-6 border-white absolute top-full left-1/2 transform -translate-1/2">
        </div>

        <div class="px-6 pt-20 pb-6">
            <h2 class="font-bold text-gray-800 text-2xl mb-2">{{ name }}</h2>
            <h3 class="text-gray-600 text-lg">{{ subheading }}</h3>
        </div>

        <div class="p-6 border-t border-gray-200 flex item-center justify-center gap-6">
            <div>
                <h4 class="text-gray-600 text-sm">Follower</h4>
                <p class="font-bold text-gray-800 text-2xl">{{ followers }}</p>
            </div>
            <div>
                <h4 class="text-gray-600 text-sm">Following</h4>
                <p class="font-bold text-gray-800 text-2xl">{{ following }}</p>
            </div>
            <div>
                <h4 class="text-gray-600 text-sm">Projects</h4>
                <p class="font-bold text-gray-800 text-2xl">{{ projects }}</p>
            </div>
        </div>
    </div>
</template>

<style scoped></style>