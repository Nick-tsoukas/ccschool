<template>
  <footer class="bg-gray-900 text-white py-12">
    <div class="container mx-auto px-6 lg:px-8">
      <!-- Top Section -->
      <div class="flex flex-col lg:flex-row lg:justify-between lg:items-center">
        <!-- Logo and Description -->
        <div class="mb-8 lg:mb-0 lg:w-1/3">
          <NuxtLink to="/" class="inline-flex items-center">
            <img
              class="h-12 w-12 rounded-full"
              src="https://picsum.photos/100"
              alt="Creativity Community School"
            />
            <span class="ml-4 text-xl font-semibold">
              Creativity Community School
            </span>
          </NuxtLink>
          <p class="mt-4 text-gray-400">
            Inspiring creativity, collaboration, and leadership for a brighter future.
          </p>
        </div>

        <!-- Navigation Links -->
        <nav class="lg:w-1/3">
          <ul class="flex flex-col gap-4 lg:flex-row lg:justify-center lg:gap-8">
            <li>
              <NuxtLink to="/" class="hover:underline">
                Home
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/about" class="hover:underline">
                About
              </NuxtLink>
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
              <NuxtLink to="/partnership" class="hover:underline">
                Partnership
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/contact" class="hover:underline">
                Contact
              </NuxtLink>
            </li>
          </ul>
        </nav>
      </div>

      <!-- Bottom Section -->
      <div class="mt-8 border-t border-gray-700 pt-6 text-center">
        <p class="text-sm text-gray-400">
          © 2024 Creativity Community School. All rights reserved.
        </p>
      </div>
    </div>
  </footer>
</template>

<script setup>
// No additional logic needed for this footer
</script>

<style scoped>
/* Add any custom styles here if necessary */
</style>
