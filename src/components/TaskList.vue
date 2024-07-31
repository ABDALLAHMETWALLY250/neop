<!-- src/components/TaskList.vue -->
<template>
  <div class="container mt-5">
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
    <h2>Task List</h2>
    <ul class="list-group">
      <TaskItem
        v-for="task in taskStore.tasks"
        :key="task.id"
        :task="task"
        :editTask="editTask"
        :toggleCompletion="toggleCompletion"
      />
    </ul>
    <hr />
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";
import { useTaskStore } from "@/store/taskStore";
import TaskItem from "./TaskItem.vue";

const taskStore = useTaskStore();
const newTask = ref("");

const addTask = async () => {
  if (newTask.value.trim()) {
    await taskStore.addTask({
      name: newTask.value,
      completed: false,
    });
    newTask.value = "";
  }
};

const editTask = (task) => {
  const newName = prompt("Edit task:", task.name);
  if (newName !== null) {
    taskStore.editTask({ ...task, name: newName });
  }
};

const toggleCompletion = (id) => {
  taskStore.toggleTaskCompletion(id);
};

// const tasks = computed(() => taskStore.tasks);

onMounted(() => {
  taskStore.fetchTasks();
});
</script>
