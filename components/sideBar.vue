<template>
  <!-- Sidebar -->
  <div
    class="bg-[#00072D] text-white flex flex-col items-center p-6 md:p-8 lg:p-12 h-full w-full md:w-64 fixed md:static top-0 z-20"
  >
    <img
      src="/profileImage.jpeg"
      alt="profile-image"
      class="w-28 h-28 rounded-full object-cover mb-6"
    />
    <!-- Navigation Links -->
    <nuxt-link to="#" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Home</nuxt-link>
    <nuxt-link to="#about" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">About</nuxt-link>
    <nuxt-link to="#projects" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Projects</nuxt-link>
    <nuxt-link to="#services" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Services</nuxt-link>
    <nuxt-link to="#contact" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Contact</nuxt-link>

    <!-- Social Icons at Bottom -->
    <div class="mt-auto flex space-x-4 pt-6">
      <a
        href="https://github.com/Nellybii"
        target="_blank"
        rel="noopener noreferrer"
        class="text-white hover:text-[#ce5a16] transition-colors"
      >
        <GithubIcon class="w-6 h-6" />
      </a>

      <a
        href="https://www.linkedin.com/in/nelly-chepkemoi-6b06951a0/"
        target="_blank"
        rel="noopener noreferrer"
        class="text-white hover:text-[#ce5a16] transition-colors"
      >
        <LinkedinIcon class="w-6 h-6" />
      </a>
    </div>
  </div>
</template>



<script setup lang="ts">
import { GithubIcon, LinkedinIcon } from 'lucide-vue-next'
</script>

