<template>
  <div>
    <button @click="toggleMessage">Show/Hide</button>
    <p v-if="showMessage">{{ message }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: "I don't even know you, Vue...",
      showMessage: true,
    };
  },
  methods: {
    toggleMessage() {
      this.showMessage = !this.showMessage;
    },
  },
};
</script>

<style>
p,
button {
  color: brown;
  border: groove;
  width: 33vw;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
  padding: 20px;
}

div {
  display: grid;
  justify-content: center;
  align-items: center;
}
</style>
