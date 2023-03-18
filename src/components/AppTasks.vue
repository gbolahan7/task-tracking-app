<template>
  <div :key="task.id" v-for="task in tasks">
    <AppTask :task="task" />
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
};
</script>
