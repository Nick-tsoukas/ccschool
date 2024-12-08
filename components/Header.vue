<template>
  <div class="bg-white">
    <header class="absolute inset-x-0 top-0 z-50">
      <div class="mx-auto max-w-7xl">
        <div class="px-6 pt-6 lg:max-w-2xl lg:pl-8 lg:pr-0">
          <nav class="flex items-center justify-between lg:justify-start" aria-label="Global">
            <NuxtLink to="/" class="-m-1.5 p-1.5">
              <span class="sr-only">Creativity Community School</span>
              <img
                alt="Creativity Community School"
                class="h-20 w-auto absolute top-4 left-4 rotate-180"
                src="@/assets/logoschool.svg"
              />
            </NuxtLink>
            <button
              type="button"
              class="-m-2.5 rounded-md p-2.5 text-gray-700 lg:hidden"
              @click="mobileMenuOpen = true"
            >
              <span class="sr-only">Open main menu</span>
              <Bars3Icon class="size-6" aria-hidden="true" />
            </button>
            <div class="hidden xl:ml-12 xl:flex xl:gap-x-14">
              <NuxtLink
                v-for="item in navigation"
                :key="item.name"
                :to="item.href"
                class="text-sm/6 font-semibold text-gray-900"
              >
                {{ item.name }}
              </NuxtLink>
            </div>
          </nav>
        </div>
      </div>
      <Dialog class="lg:hidden" @close="mobileMenuOpen = false" :open="mobileMenuOpen">
        <div class="fixed inset-0 z-50" />
        <DialogPanel
          class="fixed inset-y-0 right-0 z-50 w-full overflow-y-auto bg-white px-6 py-6 sm:max-w-sm sm:ring-1 sm:ring-gray-900/10"
        >
          <div class="flex items-center justify-between">
            <NuxtLink to="/" class="-m-1.5 p-1.5">
              <span class="sr-only">Creativity Community School</span>
              <img
                class="h-8 w-auto"
                 src="@/assets/logoschool.svg"
                alt=""
              />
            </NuxtLink>
            <button
              type="button"
              class="-m-2.5 rounded-md p-2.5 text-gray-700"
              @click="mobileMenuOpen = false"
            >
              <span class="sr-only">Close menu</span>
              <XMarkIcon class="size-6" aria-hidden="true" />
            </button>
          </div>
          <div class="mt-6 flow-root">
            <div class="-my-6 divide-y divide-gray-500/10">
              <div class="space-y-2 py-6">
                <NuxtLink
                  v-for="item in navigation"
                  :key="item.name"
                  :to="item.href"
                  class="-mx-3 block rounded-lg px-3 py-2 text-base/7 font-semibold text-gray-900 hover:bg-gray-50"
                >
                  {{ item.name }}
                </NuxtLink>
              </div>
              <div class="py-6">
                <NuxtLink
                  to="/login"
                  class="-mx-3 block rounded-lg px-3 py-2.5 text-base/7 font-semibold text-gray-900 hover:bg-gray-50"
                >
                  Log in
                </NuxtLink>
              </div>
            </div>
          </div>
        </DialogPanel>
      </Dialog>
    </header>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { Dialog, DialogPanel } from "@headlessui/vue";
import { Bars3Icon, XMarkIcon } from "@heroicons/vue/24/outline";


const navigation = [
  { name: "Home", href: "/" },
  { name: "About", href: "/about" },
  { name: "Community", href: "/community" },
  { name: "Creativity", href: "/creativity" },
  { name: "Partnership", href: "/partnership" },
  { name: "Contact", href: "/contact" },
];

const mobileMenuOpen = ref(false);
</script>
