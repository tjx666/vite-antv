<template>
  <a-button @click="increment">{{ count }}</a-button>
</template>

<script lang="ts">
import { ref, onMounted, defineComponent } from 'vue';

export default defineComponent({
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
  },
  mounted() {
    const hello = 'hello ';
    const world = 'world';

    console.log(`${hello}${world}`);
  },
});
</script>

<style></style>
