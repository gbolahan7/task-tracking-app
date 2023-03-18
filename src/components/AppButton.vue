<template>
  <button @click="onClick()" class="btn" :style="{ 'background-color': color }">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "AppButton",
  props: {
    text: String,
    color: String,
  },

  methods: {
    onClick() {},
  },
};
</script>
