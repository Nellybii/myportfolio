<template>
  <div class="max-w-7xl mx-auto py-20 px-4 md:px-8">
    <div class="grid grid-cols-1 md:grid-cols-2 gap-12">
      
      <!-- Left Column -->
      <div>
        <h2 class="text-4xl font-bold text-[#141110] border-l-4 border-[#ce5a16] pl-4 mb-2">CONTACT ME</h2>
        <p class="text-gray-600 text-lg mb-10">Get in touch with me</p>

        <div class="space-y-4 text-gray-800 text-base">
          <p><strong>Address:</strong> Nairobi, Kenya</p>
          <p><strong>Email:</strong> <a href="mailto:nellychepkem2015@gmail.com" class="text-[#ce5a16] hover:underline">nellychepkem2015@gmail.com</a></p>
          <p><strong>Phone:</strong> <a href="tel:+254706553702" class="text-[#ce5a16] hover:underline">+254 706 553 702</a></p>
          <p><strong>Website:</strong> <a href="https://github.com/Nellybii" target="_blank" class="text-[#ce5a16] hover:underline">www.github.com/Nellybii</a></p>
        </div>
      </div>

      <!-- Right Column: Form -->
      <form class="space-y-6 w-full">
        <div>
          <label for="name" class="block mb-1 font-medium text-[#141110]">Your Name</label>
          <input
            type="text"
            id="name"
            placeholder="Your Name"
            class="w-full border-b-2 border-gray-400 focus:outline-none focus:border-[#ce5a16] px-2 py-2 bg-transparent"
          />
        </div>

        <div>
          <label for="email" class="block mb-1 font-medium text-[#141110]">Your Email</label>
          <input
            type="email"
            id="email"
            placeholder="Your Email"
            class="w-full border-b-2 border-gray-400 focus:outline-none focus:border-[#ce5a16] px-2 py-2 bg-transparent"
          />
        </div>

        <div>
          <label for="message" class="block mb-1 font-medium text-[#141110]">Your Message</label>
          <textarea
            id="message"
            rows="5"
            placeholder="Your Message"
            class="w-full border-b-2 border-gray-400 focus:outline-none focus:border-[#ce5a16] px-2 py-2 bg-transparent resize-none"
          ></textarea>
        </div>

        <button
          type="submit"
          class="bg-[#ce5a16] text-white px-6 py-3 font-semibold rounded-md shadow-md hover:bg-[#b74d13] transition flex items-center justify-center gap-2"
        >
          <svg xmlns="http://www.w3.org/2000/svg" class="w-5 h-5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 4v16h16V4H4zm4 4h8m-4 8v-4m0 0l-2 2m2-2l2 2" />
          </svg>
          Send Message
        </button>
      </form>
    </div>
  </div>
</template>
