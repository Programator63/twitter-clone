<script setup lang="ts">
import useTailwindConfig from "~/composables/UseTailwindConfig";

const {defaultTransition} = useTailwindConfig()
</script>

<template>
  <NuxtLink to="#" class="flex items-center justify-center p-3 w-min hover:bg-gray-200" :class="defaultTransition">
    <div>
      <slot name="icon" class="w-6 h-6" />
    </div>
    <div>
      <slot name="name"/>
    </div>
  </NuxtLink>
</template>

<style scoped>

</style>