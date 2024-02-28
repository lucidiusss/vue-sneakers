<script setup>
defineProps({
  title: String,
  description: String,
  imageUrl: String
})

const emit = defineEmits(['closeDrawer'])
</script>

<template>
  <div class="flex flex-col items-center text-center w-72 mx-auto">
    <img height="120" width="120" :src="imageUrl" alt="Info Image" />
    <h2 class="mt-4 text-2xl font-medium">{{ title }}</h2>
    <p class="text-gray-400 mt-2">{{ description }}</p>
    <!-- <div class="relative mt-10">
      <svg
        class="absolute top-[18px] left-6 opacity-30 cursor-pointer rotate-180 transition"
        width="16"
        height="14"
        viewBox="0 0 16 14"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M1 7H14.7143"
          stroke="white"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M8.71436 1L14.7144 7L8.71436 13"
          stroke="white"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
      <button
        @click="emit('closeDrawer')"
        class="bg-lime-500 hover:bg-lime-600 active:bg-lime-700 transition px-12 py-3 text-white rounded-2xl"
      >
        Вернуться назад
      </button>
    </div> -->
  </div>
</template>
