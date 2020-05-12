<template>
  <div>
    <div
      class="relative h-screen w-screen bg-cover bg-center shadow-2xl"
      :style="`background-image:url(${bg})`"
    >
      <div class="h-screen w-screen bg-green-800 opacity-75" />
      <div
        class="absolute h-screen w-screen top-0 flex flex-col justify-center items-center"
      >
        <h1
          class="text-6xl font-bold text-white px-4 hover:bg-white hover:text-red-800 opacity-75"
        >
          Brenda Franco
        </h1>
        <h3
          class="text-3xl font-bold text-white px-4 hover:bg-white hover:text-red-800 opacity-75"
        >
          Computer Maintenance and Computer Specialist
        </h3>
      </div>
    </div>
  </div>
</template>

<script>
import bg from '../assets/bg.png'

export default {
  name: 'Home',
  data() {
    return {
      bg
    }
  }
}
</script>
