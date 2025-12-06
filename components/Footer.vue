<template>
  <footer class="bg-gray-900 text-white py-12 w-full">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Top Section -->
      <div
        class="flex flex-col gap-8 lg:flex-row lg:items-start lg:justify-between"
      >
        <!-- Logo and Description -->
        <div class="lg:w-1/3">
          <NuxtLink to="/" class="inline-flex items-center">
            <img
              class="h-12 w-12 rounded-full"
              src="@/assets/greenlogo.png"
              alt="Creativity Community School"
            />
            <span class="ml-4 text-xl font-semibold">
              Creativity Community School
            </span>
          </NuxtLink>
          <p class="mt-4 text-gray-400">
            Preparing students to be compassionate community leaders who drive
            positive change in Milwaukee and beyond.
          </p>
        </div>

        <!-- Navigation Links -->
        <nav class="lg:w-1/2">
          <ul
            class="flex flex-wrap gap-x-6 gap-y-3 justify-start lg:justify-center"
          >
            <li>
              <NuxtLink to="/" class="hover:underline">Home</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/about" class="hover:underline">About</NuxtLink>
            </li>
            <li>
              <NuxtLink to="/community" class="hover:underline">
                Community
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/creativity" class="hover:underline">
                Creativity
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/collaboration" class="hover:underline">
                Collaboration
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/contact" class="hover:underline">
                Contact
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/non-discrimination" class="hover:underline">
                Non-Discrimination
              </NuxtLink>
            </li>
          </ul>
        </nav>
      </div>

      <!-- Bottom Section -->
      <div class="mt-8 border-t border-gray-700 pt-6">
        <div class="text-center">
          <p class="text-sm text-gray-400">
            © 2024 Creativity Community School. All rights reserved.
          </p>

          <p class="mt-4 text-xs text-gray-500 max-w-3xl mx-auto">
            Creativity Community School does not discriminate on the basis of
            race, color, national origin, sex, disability, religion, sexual
            orientation, gender identity, or age in its educational programs,
            admissions, or any other school-administered programs.
            <NuxtLink
              to="/non-discrimination"
              class="ml-1 underline hover:text-gray-300"
            >
              Read our full non-discrimination policy.
            </NuxtLink>
          </p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
// nothing extra here
</script>

<style scoped>
/* no special styles needed; Tailwind handles layout */
</style>
