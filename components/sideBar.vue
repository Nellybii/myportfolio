<template>
  <div
    class="bg-[#00072D] text-white flex flex-col items-center p-6 md:p-8 lg:p-12
           h-full w-64 fixed top-0 left-0 z-30 transition-transform duration-300 ease-in-out
           transform md:translate-x-0"
    :class="{ '-translate-x-full': !isOpen }"
  >
    <img
      src="/profileImage.jpeg"
      alt="profile"
      class="w-28 h-28 rounded-full object-cover mb-6"
    />

    <nuxt-link to="#" class="my-2 hover:text-blue-400 text-xl md:text-2xl">Home</nuxt-link>
    <nuxt-link to="#about" class="my-2 hover:text-blue-400 text-xl md:text-2xl">About</nuxt-link>
    <nuxt-link to="#projects" class="my-2 hover:text-blue-400 text-xl md:text-2xl">Projects</nuxt-link>
    <nuxt-link to="#services" class="my-2 hover:text-blue-400 text-xl md:text-2xl">Services</nuxt-link>
    <nuxt-link to="#contact" class="my-2 hover:text-blue-400 text-xl md:text-2xl">Contact</nuxt-link>

    <div class="mt-auto flex space-x-4 pt-6">
      <a href="https://github.com/Nellybii" target="_blank" class="hover:text-[#ce5a16]">
        <GithubIcon class="w-6 h-6" />
      </a>
      <a href="https://linkedin.com/in/nelly-chepkemoi-6b06951a0" target="_blank" class="hover:text-[#ce5a16]">
        <LinkedinIcon class="w-6 h-6" />
      </a>
    </div>
  </div>
</template>

<script setup lang="ts">
import { GithubIcon, LinkedinIcon } from 'lucide-vue-next'
defineProps<{ isOpen: boolean }>()
</script>
