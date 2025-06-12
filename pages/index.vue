<script setup lang="ts">
import About from './about.vue'
import Projects from './projects.vue'
import Services from './services.vue'
import Contact from './contact.vue'
import Skills from './skills.vue'
</script>

<template>
  <div class="flex flex-col md:flex-row min-h-screen text-white">
    <div class="w-full md:w-64 md:fixed md:h-screen z-10 bg-[#141110]">
      <sideBar />
    </div>

    <div class="flex-1 md:ml-64 overflow-y-auto">
      <section class="flex flex-col items-center justify-center min-h-screen px-4 bg-[url('/bgImage.jpg')] bg-cover bg-center text-center">
        <img
          src="/profileImage.jpeg"
          alt="profile-image"
          class="w-36 h-36 sm:w-48 sm:h-48 rounded-full object-cover mb-6 shadow-lg"
        />
        <h1 class="text-4xl sm:text-5xl md:text-6xl font-bold text-[#ce5a16] mt-4">Nelly Chepkemoi</h1>
        <p class="text-xl sm:text-2xl md:text-3xl text-gray-300 mt-2">I'm a passionate Full Stack Developer.</p>
      </section>

      <section id="about" class="bg-[#d5d5d9] py-16 px-4 sm:px-8 md:px-16 text-black">
        <About />
      </section>

      <section id="projects" class="bg-[#c8c8d7] py-16 px-4 sm:px-8 md:px-16 text-black">
        <Projects />
      </section>

      <section id="skills" class="bg-[#c8c8d7] py-16 px-4 sm:px-8 md:px-16 text-black">
        <Skills />
      </section>

      <section id="services" class="bg-[#c5c5ca] py-16 px-4 sm:px-8 md:px-16 text-black">
        <Services />
      </section>

      <section id="contact" class="bg-[#bbbbcb] py-16 px-4 sm:px-8 md:px-16 text-black">
        <Contact />
      </section>
    </div>
  </div>
</template>
