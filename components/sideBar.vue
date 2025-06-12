<template>
  <div
    class="bg-[#00072D] text-white flex flex-col items-center p-6 md:p-8 lg:p-12 h-full w-full md:w-64 fixed md:static top-0 z-20"
  >
    <img
      src="/profileImage.jpeg"
      alt="profile-image"
      class="w-28 h-28 rounded-full object-cover mb-6"
    />
    <nuxt-link to="#" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Home</nuxt-link>
    <nuxt-link to="#about" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">About</nuxt-link>
    <nuxt-link to="#projects" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Projects</nuxt-link>
    <nuxt-link to="#services" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Services</nuxt-link>
    <nuxt-link to="#contact" class="my-2 hover:text-blue-400 text-xl md:text-2xl transition-colors">Contact</nuxt-link>
  </div>
</template>
