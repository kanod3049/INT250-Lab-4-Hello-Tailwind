<script setup>
  import ProfileCard from './components/profileCard.vue';
</script>

<template>
  <div class="flex flex-wrap items-center justify-center gap-8 min-h-screen p-8 bg-gradient-to-br from-green-500 to-sky-400">
    
    <ProfileCard 
      background="/background1.jpg" 
      profileimg="/profile1.png" 
      name="Kanokpon Suebyam" 
      subheading="Student, 20, BKK" 
      followers="482" 
      following="470" 
      projects="2"
      facebook="https://www.facebook.com/kanokpon.suebyam.908/"
      instagram="https://www.instagram.com/k_nodpok/"
    />

    <ProfileCard 
      background="/background2.jpg" 
      profileimg="/profile2.png" 
      name="Thanasorn Dusadeeroj" 
      subheading="Student, 20, BKK" 
      followers="1.2k" 
      following="300" 
      projects="5"
      facebook="https://www.facebook.com/thanasorn.dujsadeeroj.7"
      instagram="#"
    />

    <ProfileCard 
      background="/background3.jpg" 
      profileimg="/profile3.jpg" 
      name="Siriyakon Sangkaew" 
      subheading="Student, 20, BKK" 
      followers="5.8k" 
      following="1.1k" 
      projects="24"
      facebook="https://www.facebook.com/thanasorn.dujsadeeroj.7"
      instagram="#"
    />

  </div>
</template>

<style scoped></style>