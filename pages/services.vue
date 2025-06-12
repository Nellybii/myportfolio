<template>
  <div class="max-w-7xl mx-auto px-4 py-12">
    <h2 class="text-4xl font-bold text-[#141110] border-l-4 border-[#ce5a16] pl-4 mb-10">
      Services
    </h2>

    <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
      <div
        v-for="(service, index) in services"
        :key="index"
        class="bg-white shadow-md rounded-lg p-8 hover:shadow-lg transition-shadow duration-300"
      >
        <component
          :is="service.icon"
          class="h-10 w-10 text-[#ce5a16] mb-4"
        />
        <h3 class="text-xl font-semibold text-[#141110] mb-2">
          {{ service.title }}
        </h3>
        <p class="text-gray-700 text-sm leading-relaxed">
          {{ service.description }}
        </p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import {
  LaptopIcon,
  BotIcon,
  CodeIcon,
  CloudIcon,
  FileTextIcon,
  PlugZapIcon,
} from 'lucide-vue-next'

const services = [
  {
    title: 'Full Stack Development',
    description:
      'Building responsive and scalable web apps using React, Node.js, Flask, Django & more.',
    icon: LaptopIcon,
  },
  {
    title: 'AI and Automation Solutions',
    description:
      'Integration of OpenAI tools for intelligent systems, automated tasks & dashboards.',
    icon: BotIcon,
  },
  {
    title: 'Backend API Development',
    description:
      'Creating RESTful APIs with Node.js and Python, optimized for performance and security.',
    icon: CodeIcon,
  },
  {
    title: 'Cloud Deployment',
    description:
      'Deploying apps on Azure, Vercel, and other cloud platforms with production-readiness.',
    icon: CloudIcon,
  },
  {
    title: 'Technical Documentation',
    description:
      'Clear and structured user guides, developer manuals, and internal documentation.',
    icon: FileTextIcon,
  },
  {
    title: 'API & Third-party Integration',
    description:
      'Connecting apps to third-party APIs: payments, analytics, storage & more.',
    icon: PlugZapIcon,
  },
]
</script>
