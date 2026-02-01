<script setup>
    defineProps([
        "profileimg",
        "background",
        "name",
        "subheading",
        "followers",
        "following",
        "projects",
        "facebook",  
        "instagram", 
        "linkedin" 
    ]);
</script>

<template>
    <div class="bg-white shadow-lg rounded-2xl w-80 overflow-hidden text-center transition-all duration-300 hover:-translate-y-2 hover:shadow-2xl">
        
        <!-- Background Header -->
        <div class="relative h-32 bg-cover bg-center" :style="'background-image: url(' + background + ')'">
            <!-- Profile Image -->
            <img :src="profileimg" alt="Profile" 
                 class="inline-block w-24 h-24 rounded-full object-cover border-4 border-white absolute top-20 left-1/2 transform -translate-x-1/2 shadow-sm">
        </div>

        <!-- Content Section -->
        <div class="px-6 pt-14 pb-4">
            <h2 class="font-bold text-gray-800 text-xl mb-1">{{ name }}</h2>
            <p class="text-gray-500 text-sm mb-4">{{ subheading }}</p>

            <div class="flex justify-center gap-4 mb-2">
                <a v-if="facebook" :href="facebook" target="_blank" class="text-blue-600 hover:text-blue-800 text-xs font-semibold">Facebook</a>
                <a v-if="instagram" :href="instagram" target="_blank" class="text-pink-600 hover:text-pink-800 text-xs font-semibold">Instagram</a>
            </div>
        </div>

        <!-- Stats Section -->
        <div class="p-4 border-t border-gray-100 flex items-center justify-around bg-gray-50/50">
            <div>
                <p class="font-bold text-gray-800 text-lg">{{ followers }}</p>
                <h4 class="text-gray-500 text-[10px] uppercase tracking-wider">Followers</h4>
            </div>
            <div>
                <p class="font-bold text-gray-800 text-lg">{{ following }}</p>
                <h4 class="text-gray-500 text-[10px] uppercase tracking-wider">Following</h4>
            </div>
            <div>
                <p class="font-bold text-gray-800 text-lg">{{ projects }}</p>
                <h4 class="text-gray-500 text-[10px] uppercase tracking-wider">Projects</h4>
            </div>
        </div>
    </div>
</template>

<style scoped></style>