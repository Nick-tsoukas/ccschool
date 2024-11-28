<template>
  <div class="bg-gray-50 py-16 sm:py-24">
    <div class="container mx-auto px-6 lg:px-8">
      <!-- Page Header -->
      <div class="text-center">
        <h1 class="text-5xl font-bold text-gray-900">Partner With Us</h1>
        <p class="mt-6 text-lg text-gray-700">
          Join us in shaping the future of education. Your involvement can make a meaningful difference in our community.
        </p>
      </div>

      <!-- Get Involved Section -->
      <div class="mt-16 grid grid-cols-1 gap-y-12 lg:grid-cols-2 lg:gap-x-16">
        <!-- Volunteer Section -->
        <div>
          <h2 class="text-3xl font-semibold text-gray-900">Volunteer</h2>
          <p class="mt-4 text-gray-700">
            Share your time and talents to support our mission. Whether you’re helping in classrooms, mentoring students,
            or assisting with events, your efforts play a vital role in creating a positive impact.
          </p>
        </div>

        <!-- Donate Section -->
        <div>
          <h2 class="text-3xl font-semibold text-gray-900">Donate</h2>
          <p class="mt-4 text-gray-700">
            Your generosity helps us provide resources, programs, and opportunities that empower our students to succeed.
            Every contribution, big or small, makes a difference.
          </p>
          <div class="mt-6">
            <button
              type="button"
              class="rounded-md bg-indigo-600 px-6 py-3 text-white font-semibold shadow-sm hover:bg-indigo-500 focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:ring-offset-2"
            >
              Donate Now
            </button>
          </div>
        </div>
      </div>

      <!-- Call-to-Action -->
      <div class="mt-16 text-center">
        <h2 class="text-3xl font-semibold text-gray-900">Ready to Get Involved?</h2>
        <p class="mt-4 text-gray-700">
          Contact us to learn more about how you can support our mission and be part of our community.
        </p>
        <div class="mt-6">
          <NuxtLink
            to="/contact"
            class="rounded-md bg-gray-900 px-6 py-3 text-white font-semibold shadow-sm hover:bg-gray-800 focus:outline-none focus:ring-2 focus:ring-gray-800 focus:ring-offset-2"
          >
            Contact Us
          </NuxtLink>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// No additional logic needed
</script>

<style scoped>
/* Add any custom styles here if needed */
</style>
