<template>
  <div class="flex items-center justify-center p-4">
    <AnimateGrid :cards :rotateY="0" :rotateX="0">
      <template #logo="{ logo }">
        <img
          class="logo mx-auto h-30 w-auto"
          :src="logo"
        />
      </template>
    </AnimateGrid>
  </div>
</template>

<script lang="ts" setup>

const cards = Array.from({ length: 16 }, () => ({
  logo: '/images/avatars/Alex-2.png',
}));
</script>