<template>
  <div class="counter-wrapp">
    <h1 class="counter">{{ count }}</h1>
    <div class="buttons">
      <button class="counter-btn1" @click="inc">+1</button>
      <button class="counter-btn2" @click="reset">reset</button>
    </div>
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
    reset() {
      this.count = 0;
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
.buttons {
  display: flex;
  gap: 20px;
}

/* button-first */
.counter-btn1 {
  font-weight: 900;
  padding: 10px 24px 10px;
  font-size: 12px;
  border-radius: 10px;
  border: blue;
  background-color: blue;
  color: azure;
}
.counter-btn1:hover {
  border: 1px solid #fff;
  background-color: #fff;
  color: black;
}

/* button-twщ */
.counter-btn2 {
  font-weight: 900;
  padding: 10px 24px 10px;
  font-size: 12px;
  border-radius: 10px;
  border: red;
  background-color: red;
  color: azure;
}
.counter-btn2:hover {
  border: 1px solid #fff;
  background-color: #fff;
  color: black;
}
</style>
