<template>
  <div class="card">
    <p class="counter-text">Counter {{ count }}</p>
    <button @click="increment" class="btn">+</button>
    <button @click="decrement" class="btn">-</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0,
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
      if (this.count > 0) {
        this.count--;
      }
    },
  },
};
</script>

<style>
.card{}
.counter-text {
  font-size: 24px;
  font-weight: bold;
  color: #333;
}

.btn {
  padding: 10px 20px;
  font-size: 18px;
  background-color: #007BFF;
  color: #fff;
  border: none;
  margin: 5px;
  cursor: pointer;
  border-radius: 5px;
}

.btn:hover {
  background-color: #0056b3;
}
</style>
