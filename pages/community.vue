<template>
  <div class="bg-gray-50 py-16 sm:py-24">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="text-center max-w-4xl mx-auto">
        <h1 class="text-5xl font-bold text-gray-900">Our Community</h1>
        <p class="mt-6 text-lg text-gray-700">
          At Creativity Community School, we believe education goes beyond the classroom. 
          Our vibrant community of students, educators, families, and local partners work 
          together to create an inclusive and supportive environment that fosters growth, 
          collaboration, and innovation.
        </p>
      </div>
      <div class="mt-16 grid grid-cols-1 gap-y-16 lg:grid-cols-3 lg:gap-x-12">
        <div v-for="section in sections" :key="section.title" class="text-center">
          <img :src="section.image" :alt="section.title" class="w-20 h-20 mx-auto mb-6 rounded-full object-cover" />
          <h2 class="text-2xl font-semibold text-gray-900">{{ section.title }}</h2>
          <p class="mt-4 text-gray-700">{{ section.description }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const sections = [
  {
    title: "Engaged Students",
    description: "Our students are active participants in their own learning, exploring new ideas and collaborating on meaningful projects.",
    image: "https://picsum.photos/80?random=1",
  },
  {
    title: "Dedicated Educators",
    description: "Our teachers are passionate about guiding students through hands-on experiences that spark curiosity and inspire growth.",
    image: "https://picsum.photos/80?random=2",
  },
  {
    title: "Community Partners",
    description: "We collaborate with local businesses and organizations to provide real-world opportunities for students to learn and thrive.",
    image: "https://picsum.photos/80?random=3",
  },
];
</script>

<style scoped>
/* Additional styles can be added here if needed */
</style>
