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
        <div
          class="flex size-full flex-col items-center justify-center"
        >
          <span
            class="gap-2 bg-gradient-to-b from-neutral-200 to-neutral-500 bg-clip-text text-center text-4xl font-bold text-transparent md:text-left md:text-6xl"
          >
            Berthold Wizard
          </span>
          <span
            class="gap-2 bg-gradient-to-b from-neutral-200 to-neutral-500 bg-clip-text text-center text-xl font-medium text-transparent md:text-left md:text-3xl"
          >
            cooming soon
          </span>
        </div>
      </div>
    </Vortex>
  </section>
</template>

<script lang="ts" setup>

</script>