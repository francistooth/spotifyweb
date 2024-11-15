<template>
  <div class="fixed bottom-0 left-0 w-full bg-black text-white shadow-lg">
    <div class="flex items-center justify-between px-4 py-2">
      <!-- Left Section: Song Info -->
      <div class="flex items-center space-x-4">
        <img
          src="https://via.placeholder.com/50"
          alt="Album Art"
          class="w-12 h-12 rounded-md"
        />
        <div>
          <h2 class="text-sm font-semibold">Song Title</h2>
          <p class="text-xs text-gray-400">Artist Name</p>
        </div>
      </div>

      <!-- Center Section: Controls -->

      <div class="flex flex-col items-center space-y-2">
        <div class="flex items-center space-x-4">
          <button>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 text-gray-400 hover:text-white"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="1"
                d="M10 9l-6 3 6 3V9z"
              />
            </svg>
          </button>

          <!-- Play/Pause Button -->

          <button class="bg-white hover:bg-gray-200 p-2 rounded-full">
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-6 w-6 text-black"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M5 3v18l15-9L5 3z"
              />
            </svg>
          </button>
          <button>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              class="h-5 w-5 text-gray-400 hover:text-white"
              fill="none"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path
                stroke-linecap="round"
                stroke-linejoin="round"
                stroke-width="2"
                d="M14 5l6 5-6 5V5z"
              />
            </svg>
          </button>
        </div>


        <!-- Progress Bar -->


        <div class="w-64">
          <input
            type="range"
            min="0"
            max="100"
            value="50"
            class="w-full appearance-none bg-gray-600 h-1 rounded-lg"
          />
          <div class="flex justify-between text-xs text-gray-400 mt-1">
            <span>1:12</span>
            <span>3:45</span>
          </div>
        </div>
      </div>

      <!-- Right Section: Volume -->

      
      <div class="flex items-center space-x-2">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5 text-gray-400 hover:text-white"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M11 5L6 9H2v6h4l5 4V5z"
          />
        </svg>
        <input
          type="range"
          min="0"
          max="100"
          value="70"
          class="w-24 appearance-none bg-gray-600 h-1 rounded-lg"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Player",
};
</script>

<style scoped>
/* Optional: Add custom styles if needed */
</style>
