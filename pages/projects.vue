<template>
  <div class="py-12 px-4 md:px-12">
    <div class="mb-12 text-left">
      <h2 class="text-4xl font-bold text-[#141110] border-l-4 border-[#ce5a16] pl-4 mb-2">PROJECTS</h2>
        <p class="text-gray-600 text-lg mb-10">Check out my below Projects Completed and others on my github .Have more than 6 projects done both for companies and individual clients.Click this link <a href="https://github.com/Nellybii" target="_blank" class="text-[#1873da] hover:underline">GitHub Profile</a> </p>
    </div>

    <div class="space-y-14">
      <div
        v-for="project in projects"
        :key="project.title"
        class="flex flex-col md:flex-row gap-6 border border-[#ce5a16] rounded-lg shadow-lg overflow-hidden"
      >
        <!-- Project Image -->
        <img
          :src="project.image"
          :alt="project.title"
          class="w-full md:w-1/2 h-64 object-cover"
        />

        <!-- Project Content -->
        <div class="flex flex-col justify-between p-6 w-full">
          <div>
            <h2 class="text-2xl font-semibold text-[#141110] mb-2">{{ project.title }}</h2>
            <p class="text-gray-700 mb-4">{{ project.description }}</p>
          </div>
          <div class="mt-4">
            <a
              :href="project.link"
              target="_blank"
              class="bg-[#ce5a16] text-white font-medium px-6 py-2 rounded hover:bg-[#a94610] transition"
            >
              Live Link
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          title: 'Journaling App',
          description: 'A journaling platform built using Node.js, PostgreSQL, and ReactJS. Users can log and track their journal entries.',
          image: 'https://images.unsplash.com/photo-1524995997946-a1c2e315a42f?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=600',
          link: 'https://journals-entry.vercel.app/'
        },
        {
          title: 'Portfolio Website',
          description: 'A personal portfolio built with NuxtJS showcasing my projects, skills, and experience.',
          image: 'https://images.unsplash.com/photo-1508780709619-79562169bc64?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=600',
          link: 'https://my-portfolio-ten-red-64.vercel.app/'
        },
        {
          title: 'Furniture Garden App',
          description: 'An e-commerce platform for furniture shopping built with Flask and ReactJS.',
          image: 'https://images.unsplash.com/photo-1600585154340-be6161a56a0c?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=600',
          link: 'https://furniture-garden-frontend.vercel.app/'
        },
        {
          title: 'Job Listing App',
          description: 'A job listing app using Node.js, Express, ReactJS, and MongoDB with full CRUD functionality and third-party API integrations.',
          image: 'https://images.unsplash.com/photo-1557425529-b1ae9c141e7d?crop=entropy&cs=tinysrgb&fit=max&fm=jpg&q=80&w=600',
          link: 'https://lysterpro.vercel.app/'
        }
      ]
    };
  }
};
</script>
