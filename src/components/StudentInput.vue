<template>
  <div>
    <p v-for="student in students" :key="student.id">{{ student.name }}</p>
  </div>
</template>

<script lang="ts">
import { defineComponent, reactive, computed } from 'vue';

interface Student {
  id: number;
  name: string;
  grade: string;
}

export default defineComponent({
  name: 'StudentComponent',
  setup() {
    const state = reactive({
      students: [
        { id: 1, name: 'John Doe', grade: 'A' },
        { id: 2, name: 'Jane Doe', grade: 'B' },
        { id: 3, name: 'John Smith', grade: 'C' },
        { id: 4, name: 'Jane Smith', grade: 'D' }
      ] as Student[]
    });

    const students = computed(() => state.students);

    return {
      students
    };
  }
});
</script>

<style scoped>
body {
  background-color: #f0f0f0;
  text-align: center;
  margin: 0 auto;
}
</style>
