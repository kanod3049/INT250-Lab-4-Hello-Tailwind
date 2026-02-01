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
      github="https://github.com/kanod3049"
    />

    <ProfileCard 
      background="/background2.jpg" 
      profileimg="/profile2.png" 
      name="Thanasorn Dusadeeroj" 
      subheading="Student, 20, BKK" 
      followers="634" 
      following="1,915" 
      projects="3"
      facebook="https://www.facebook.com/thanasorn.dujsadeeroj.7"
      instagram="https://www.instagram.com/savaki_tns/"
      github="https://github.com/vavaza09"
    />

    <ProfileCard 
      background="/background3.jpg" 
      profileimg="/profile3.jpg" 
      name="Siriyakon Sangkaew" 
      subheading="Student, 20, BKK" 
      followers="539" 
      following="851" 
      projects="3"
      facebook="https://www.facebook.com/tan.siriyagon"
      instagram="https://www.instagram.com/siri_yx/"
      github="https://github.com/SvechaZ"
    />

  </div>
</template>

<style scoped></style>