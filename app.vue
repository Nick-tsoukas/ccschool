<template>
  <div class="min-h-screen flex flex-col overflow-x-hidden">
    <Header />
    <main class="flex-1">
      <NuxtPage />
    </main>
    <Footer />
  </div>
</template>

<script setup lang="ts">
// nothing needed here
</script>

<style>
/* Optional global safety net, if you don't already have it */
html,
body {
  margin: 0;
  padding: 0;
}
</style>
