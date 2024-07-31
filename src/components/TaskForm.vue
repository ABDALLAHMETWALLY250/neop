<template>
  <form @submit.prevent="addTask">
    <div class="input-group mt-3">
      <input
        v-model="newTask"
        type="text"
        class="form-control"
        placeholder="New task"
        required
      />
      <button type="submit" class="btn btn-primary">Add Task</button>
    </div>
  </form>
</template>
  
  <script setup>
import { ref } from "vue";
import { useTaskStore } from "@/store/taskStore";

const taskStore = useTaskStore();
const newTask = ref("");

const addTask = () => {
  if (newTask.value.trim()) {
    taskStore.addTask({
      id: Date.now(),
      name: newTask.value,
      completed: false,
    });
    newTask.value = "";
  }
};
</script>
  