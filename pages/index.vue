<template>
  <div class="bg-white">
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
              <h2 class=" italic  text-xl my-4 font-bold tracking-tight text-gray-900 sm:text-xl">
                Milwaukee’s first Project Based Middle & High School
              </h2>
              <p class="mt-8 text-pretty text-lg font-medium text-gray-950 sm:text-lg/8">
                At Creativity Community School education goes beyond the classroom, inspiring students to explore, innovate, and engage with real-world challenges.
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
          src="@/assets/millwaukeenew.jpg"
          alt="Milwaukee cityscape"
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
      <img :src="feature.image" :alt="feature.name" class="min-h-[480px] w-full object-cover" />
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

import communityImage from "@/assets/garden.png";
import creativityImage from "@/assets/handsonlearning.jpg";
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
    href: "/collaboration",
    image: partnershipImage,
  },
];

const navigation = [
  { name: "Home", href: "/" },
  { name: "About", href: "/about" },
  { name: "Community", href: "/community" },
  { name: "Creativity", href: "/creativity" },
  { name: "Collaboration", href: "/collaboration" },
  { name: "Contact", href: "/contact" },
];

const mobileMenuOpen = ref(false);
</script>
