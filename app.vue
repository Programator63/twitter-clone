<script setup lang="ts">
const darkMode = ref(false)


</script>

<template>
  <div :class="{'dark': darkMode}">
    <div class="bg-white dark:bg-dim-900">
      <div class="m-h-full">
        <div class="grid grid-cols-12 mx-auto sm:px-6 lg:m-w-7xl lg:px-8 lg:gap-8">
          <!-- Left SideBar -->
          <div class="hidden md:block xs-col-span-1 xl:col-span-1">
            <div class="sticky top-0"></div>
            <SidebarLeft/>
          </div>
          <!-- Main Content -->
          <NuxtPage/>
          <!-- Right SideBar-->
        </div>
      </div>
    </div>
  </div>
</template>
