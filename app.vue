<template>
  <section class="relative mx-auto h-screen w-full overflow-hidden">
    <Vortex
      background-color="black"
      :range-y="800"
      :particle-count="500"
      :base-hue="180"
      class="absolute inset-0 flex items-center justify-center px-8"
    >
      <div class="flex size-full max-w-6xl flex-col md:flex-row">
        <div class="m-auto flex flex-col gap-3">
          <div class="flex flex-col">
            <RadiantText
              class="inline-flex flex-col items-center justify-center px-4 py-0 transition ease-out hover:text-neutral-600 hover:duration-300 hover:dark:text-neutral-400"
              :duration="5"
            >
              <span class="text-6xl font-bold">🧙🏻‍♂️</span>
              <span class="text-3xl font-bold">Berthold Wizard</span>
              <span class="text-xs font-light">©2024 Edition</span>
            </RadiantText>
          </div>
          <div class="z-10 flex flex-col gap-2">
            <RainbowButton disabled>Spielen</RainbowButton>
            <RainbowButton disabled>Leaderboard</RainbowButton>
            <RainbowButton is="a" href="/files/anleitung.pdf">Anleitung</RainbowButton>
          </div>
          <div class="flex flex-col py-2">
            <div class="flex">
              <AnimatedTooltip :items="people" />
            </div>
            <Nuxt-Link to="/about" class="m-auto">
              <span class="font-light text-neutral-600">more</span>
            </Nuxt-Link>
          </div>
        </div>
      </div>
    </Vortex>
  </section>
</template>

<script lang="ts" setup>
const people = [
  {
    id: 1,
    name: "Alex",
    designation: "Software Engineer",
    image:
      "/images/avatars/Alex-2.png",
  },
  {
    id: 2,
    name: "Thomas",
    designation: "CTO",
    image:
      "/images/avatars/Thomas.png",
  },
  {
    id: 3,
    name: "Joachim",
    designation: "CEO",
    image:
      "/images/avatars/Joachim.png",
  },
  {
    id: 4,
    name: "Mani",
    designation: "Techniker",
    image:
      "/images/avatars/Mani.png",
  },
  {
    id: 5,
    name: "Sandro",
    designation: "Software Engineer",
    image:
      "/images/avatars/Sandro.png",
  },
  {
    id: 6,
    name: "Oliver",
    designation: "Software Engineer",
    image:
      "/images/avatars/Oliver.png",
  },
];
</script>