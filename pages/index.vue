<template>
  <div class="bg-white">
   <!-- <header class="absolute inset-x-0 top-0 z-50">
      <div class="mx-auto max-w-7xl">
        <div class="px-6 pt-6 lg:max-w-2xl lg:pl-8 lg:pr-0">
          <nav class="flex items-center justify-between lg:justify-start" aria-label="Global">
            <NuxtLink to="/" class="-m-1.5 p-1.5">
              <span class="sr-only">Creativity Community School</span>
              <img
                alt="Creativity Community School"
                class="h-8 w-auto"
                src="https://tailwindui.com/plus/img/logos/mark.svg?color=indigo&shade=600"
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
            <div class="hidden lg:ml-12 lg:flex lg:gap-x-14">
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
                src="https://tailwindui.com/plus/img/logos/mark.svg?color=indigo&shade=600"
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
    </header> -->

    <div class="relative">
      <div class="mx-auto max-w-7xl">
        <div class="relative z-10 pt-14 lg:w-full lg:max-w-2xl">
          <svg
            class="absolute inset-y-0 right-8 hidden h-full w-80 translate-x-1/2 transform fill-white lg:block"
            viewBox="0 0 100 100"
            preserveAspectRatio="none"
            aria-hidden="true"
          >
            <polygon points="0,0 90,0 50,100 0,100" />
          </svg>

          <div class="relative px-6 py-32 sm:py-40 lg:px-8 lg:py-56 lg:pr-0">
            <div class="mx-auto max-w-2xl lg:mx-0 lg:max-w-xl">
              <h1 class="text-pretty text-5xl font-bold tracking-tight text-gray-900 sm:text-7xl">
                Learn by Doing
              </h1>
              <p class="mt-8 text-pretty text-lg font-medium text-gray-950 sm:text-xl/8">
                At Creativity Community School, we inspire students through hands-on projects
                and real-world challenges, fostering creativity, collaboration, and leadership
                for a brighter future.
              </p>
              <div class="mt-10 flex items-center gap-x-6">
                <NuxtLink
                  to="/about"
                  class="rounded-md bg-indigo-600 px-3.5 py-2.5 text-sm font-semibold text-white shadow-sm hover:bg-indigo-500 focus-visible:outline focus-visible:outline-2 focus-visible:outline-offset-2 focus-visible:outline-indigo-600"
                >
                  Learn More
                </NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="bg-gray-50 lg:absolute lg:inset-y-0 lg:right-0 lg:w-1/2">
        <img
          class="aspect-[3/2] object-cover lg:aspect-auto lg:size-full"
          src="@/assets/millwaukee.png"
          alt=""
        />
      </div>
    </div>

    <!-- Features Section -->
    <div class="bg-slate-50 py-24 sm:py-32">
      <div class="mx-auto max-w-7xl px-6 lg:px-8">
        <div class="max-w-4xl lg:text-left">
          <h2 class="mt-2 text-pretty text-5xl font-semibold tracking-tight text-black sm:text-5xl lg:text-balance">
            Innovating Education
          </h2>
          <p class="mt-6 text-2xl text-black">
            At Creativity Community School, our mission is to empower students to explore
            their passions, think critically, and innovate boldly. Through experiential
            learning and a supportive community, we nurture the leaders and problem-solvers
            of tomorrow.
          </p>
        </div>
        <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-none">
          <dl class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-16 lg:max-w-none lg:grid-cols-3">
            <div
      v-for="feature in features"
      :key="feature.name"
      class="flex flex-col items-center text-center"
    >
      <img :src="feature.image" :alt="feature.name" class="" />
      <p class="text-3xl pt-6 font-semibold text-black">{{ feature.name }}</p>
      <dd class="mt-4 text-lg text-black">
        <p>{{ feature.description }}</p>
        <p class="mt-6">
          <NuxtLink :to="feature.href" class="text-sm/6 font-semibold text-indigo-400">
            Learn more <span aria-hidden="true">→</span>
          </NuxtLink>
        </p>
      </dd>
    </div>
          </dl>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { Dialog, DialogPanel } from "@headlessui/vue";
import { Bars3Icon, XMarkIcon } from "@heroicons/vue/24/outline";

// images 

import communityImage from "@/assets/community.png";
import creativityImage from "@/assets/creativity.png";
import partnershipImage from "@/assets/partnership.png";


const features = [
  {
    name: "Community",
    description:
      "Our community-driven, non-profit school is dedicated to transforming education.",
    href: "/community",
    image: communityImage,
  },
  {
    name: "Creativity",
    description:
      "We believe creativity is the key to solving tomorrow’s challenges.",
    href: "/creativity",
    image: creativityImage,
  },
  {
    name: "Partner With Us",
    description:
      "Join us in shaping the future of learning! By partnering, you can play a vital role.",
    href: "/partnership",
    image: partnershipImage,
  },
];

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
