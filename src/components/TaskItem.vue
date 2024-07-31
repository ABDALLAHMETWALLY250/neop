<!-- src/components/TaskItem.vue -->
<template>
  <li class="list-group-item d-flex justify-content-between flex-wrap gap-3 align-items-center">
    <span :class="{ completed: task.completed }">{{ task.userId }}</span>
    <span :class="{ completed: task.completed }">{{ task.title }}</span>
    <div>
      <button class="btn btn-sm btn-info mx-2" @click="editTask(task)">
        Edit
      </button>
      <button
        class="btn btn-sm btn-success mx-2"
        @click="toggleCompletion(task.id)"
      >
        {{ task.completed ? "Undo" : "Complete" }}
      </button>
      <button class="btn btn-sm btn-danger" @click="handleDelete(task.id)">
        Delete
      </button>
    </div>
  </li>
</template>

<script setup>
import { defineProps } from "vue";
import { useTaskStore } from "@/store/taskStore";

const props = defineProps(["task", "editTask", "toggleCompletion"]);

const taskStore = useTaskStore();

const handleDelete = async (id) => {
  await taskStore.deleteTask(id);
};
</script>

<style scoped>
.completed {
  text-decoration: line-through;
}
</style>
