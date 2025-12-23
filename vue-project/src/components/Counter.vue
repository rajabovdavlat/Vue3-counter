<template>
  <div class="counter-wrapp">
    <h1 class="counter">{{ count }}</h1>
    <button class="counter-btn" @click="inc">+1</button>
  </div>
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

<style scoped>
.counter-wrapp {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
}
.counter {
   font-weight: 700;
   font-size: 50px;
   color: brown;
}
.counter-btn{
    font-weight: 900;
    padding: 10px 24px 10px;
    font-size: 12px;
    border-radius: 10px;
    border: none;
    background-color: blue;
    color: azure;
}
.counter-btn:hover{
    border: 1px  solid #fff;
    background-color: #fff;
    color: black;
}
</style>
