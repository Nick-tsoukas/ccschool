<template>
  <div class="bg-gray-50 py-16 sm:py-24">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <!-- Page Header -->
      <div class="text-center max-w-4xl mx-auto">
        <h1 class="text-5xl font-bold text-gray-900">Creativity at Our Core</h1>
        <p class="mt-6 text-lg text-gray-700">
          At Creativity Community School, we believe that creativity is the spark that drives innovation and growth.
          We foster an environment where students explore, imagine, and create through hands-on projects and real-world problem solving.
        </p>
      </div>

      <!-- Content Section -->
      <div class="mt-16 grid grid-cols-1 gap-y-16 lg:grid-cols-2 lg:gap-x-12">
        <!-- First Column -->
        <div>
          <h2 class="text-3xl font-semibold text-gray-900">Why Creativity Matters</h2>
          <p class="mt-4 text-gray-700">
            Creativity is the key to unlocking human potential. By encouraging students to think outside the box,
            we empower them to tackle challenges, develop innovative solutions, and express themselves confidently.
          </p>
          <p class="mt-4 text-gray-700">
            Our curriculum is designed to ignite curiosity and enable students to learn through discovery. With
            creativity as a cornerstone of our programs, students grow into confident, resilient, and inspired individuals.
          </p>
        </div>

        <!-- Second Column -->
        <div>
          <h2 class="text-3xl font-semibold text-gray-900">How We Nurture Creativity</h2>
          <p class="mt-4 text-gray-700">
            We provide hands-on learning experiences that encourage experimentation and innovation. Through projects,
            art, and interdisciplinary challenges, students develop their creative abilities in meaningful ways.
          </p>
          <ul class="mt-4 space-y-3">
            <li class="flex items-start">
              <span class="inline-block h-6 w-6 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold">
                ✓
              </span>
              <p class="ml-3 text-gray-700">Project-Based Learning</p>
            </li>
            <li class="flex items-start">
              <span class="inline-block h-6 w-6 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold">
                ✓
              </span>
              <p class="ml-3 text-gray-700">Art and Design Opportunities</p>
            </li>
            <li class="flex items-start">
              <span class="inline-block h-6 w-6 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold">
                ✓
              </span>
              <p class="ml-3 text-gray-700">Real-World Problem Solving</p>
            </li>
            <li class="flex items-start">
              <span class="inline-block h-6 w-6 bg-indigo-500 rounded-full flex items-center justify-center text-white font-bold">
                ✓
              </span>
              <p class="ml-3 text-gray-700">Collaborative Teamwork</p>
            </li>
          </ul>
        </div>
      </div>

      <!-- Call-to-Action -->
      <div class="mt-16 text-center">
        <NuxtLink
          to="/community"
          class="inline-block rounded-md bg-indigo-600 px-6 py-3 text-white font-semibold shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
        >
          Learn More About Our Community
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
// No additional setup needed for this page
</script>

<style scoped>
/* Add any custom styles if necessary */
</style>
