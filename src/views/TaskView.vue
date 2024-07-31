<template>
  <div class="container" style="margin-top: 5rem">
    <!-- <TaskForm /> -->
    <TaskList />
  </div>
</template>

<script setup>
import TaskList from "../components/TaskList.vue";
// import TaskForm from "../components/TaskForm.vue";
</script>

<style scoped>
.completed {
  text-decoration: line-through;
}
</style>
