<template>
  <div :key="task.id" v-for="task in tasks">
    <AppTask @delete-task="$emit('delete-task', task.id)" :task="task" />
  </div>
</template>

<script>
import AppTask from "./AppTask.vue";
export default {
  name: "AppTasks",
  props: {
    tasks: Array,
  },
  components: { AppTask },
  emits: ["delete-task"],
};
</script>
