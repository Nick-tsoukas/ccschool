<template>
  <div class="bg-gray-50 py-16 sm:py-24">
    <div class="container mx-auto px-6 lg:px-8">
      <!-- Page Header -->
      <div class="text-center max-w-4xl mx-auto">
        <h1 class="text-5xl font-bold text-gray-900">About Us</h1>
        <p class="mt-6 text-lg text-gray-700">
          At Creativity Community School, we are dedicated to transforming education
          by fostering creativity, collaboration, and leadership in a supportive environment.
        </p>
      </div>

      <!-- About Content -->
      <div class="mt-16 grid grid-cols-1 gap-y-12 lg:grid-cols-2 lg:gap-x-16">
        <!-- Mission Section -->
        <div>
          <h2 class="text-3xl font-semibold text-gray-900">Our Mission</h2>
          <p class="mt-4 text-gray-700">
            Our mission is to empower students to explore their passions, think critically, and
            innovate boldly. By focusing on hands-on projects and real-world challenges, we equip
            students with the skills and confidence to make a positive impact in their communities
            and beyond.
          </p>
        </div>

        <!-- Vision Section -->
        <div>
          <h2 class="text-3xl font-semibold text-gray-900">Our Vision</h2>
          <p class="mt-4 text-gray-700">
            We envision a future where education inspires creativity and collaboration, enabling
            students to become compassionate, lifelong learners who shape a brighter future for all.
          </p>
        </div>
      </div>

      <!-- Values Section -->
      <div class="mt-16">
        <h2 class="text-center text-3xl font-semibold text-gray-900">Our Core Values</h2>
        <div class="mt-8 grid grid-cols-1 gap-y-12 sm:grid-cols-2 lg:grid-cols-3 lg:gap-x-8 lg:gap-y-16">
          <div class="text-center">
            <div class="inline-flex h-16 w-16 items-center justify-center rounded-full bg-indigo-100">
              <span class="text-indigo-600 text-3xl font-bold">💡</span>
            </div>
            <h3 class="mt-4 text-xl font-semibold text-gray-900">Creativity</h3>
            <p class="mt-2 text-gray-700">
              Encouraging innovative thinking and problem-solving to unlock potential.
            </p>
          </div>

          <div class="text-center">
            <div class="inline-flex h-16 w-16 items-center justify-center rounded-full bg-indigo-100">
              <span class="text-indigo-600 text-3xl font-bold">🤝</span>
            </div>
            <h3 class="mt-4 text-xl font-semibold text-gray-900">Collaboration</h3>
            <p class="mt-2 text-gray-700">
              Building strong connections through teamwork and shared goals.
            </p>
          </div>

          <div class="text-center">
            <div class="inline-flex h-16 w-16 items-center justify-center rounded-full bg-indigo-100">
              <span class="text-indigo-600 text-3xl font-bold">🌍</span>
            </div>
            <h3 class="mt-4 text-xl font-semibold text-gray-900">Leadership</h3>
            <p class="mt-2 text-gray-700">
              Empowering students to lead with integrity and make a difference.
            </p>
          </div>
        </div>
      </div>

      <!-- Call-to-Action -->
      <div class="mt-16 text-center">
        <NuxtLink
          to="/contact"
          class="rounded-md bg-indigo-600 px-6 py-3 text-white font-semibold shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
        >
          Get in Touch
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script setup>
// No additional logic needed for this page
</script>

<style scoped>
/* Add any custom styles if necessary */
</style>
