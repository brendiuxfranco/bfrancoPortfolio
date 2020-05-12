<template>
  <div>
    <div
      class="pt-24 min-h-screen top flex flex-col flex-wrap justify-center items-center px-8 bg-green-700 shadow-lg"
    >
      <div class="w-full flex flex-wrap">
        <div
          v-for="(project, index) in projects"
          :key="index"
          class="w-1/4 p-2"
        >
          <Card :project="project" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Card from '../components/Card'
import projects from '../data/projects'

export default {
  name: 'Portfolio',
  components: {
    Card
  },
  data() {
    return {
      projects
    }
  }
}
</script>

<style lang="scss" scoped></style>
