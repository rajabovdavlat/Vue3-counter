<template>
  <h1>{{ count }}</h1>
  <button @click="inc">+1</button>
</template>


<!-- methods Options API -->
<script>
export default {
  data() {
    return { count: 0 };
  },
  methods: {
    inc() {
      this.count++;
    },
  },
};
</script>
