<template>
  <div :id="myClass">
    <h2>Hola</h2>
    <p>{{ counter }}</p>
    <button v-on:click="counter++" :disabled="isDisabled">
      Cambiar de color
    </button>
    <button @click="isDisabled = false">Make able</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      myClass: "card",
      isDisabled: true,
      counter: 1,
    };
  },
  methods: {
    changeColor() {
      this.myClass = "card-dark";
    },
  },
};
</script>

<style>
#card {
  background: red;
  padding: 10px;
  border: 1px solid orange;
}

#card-dark {
  background: black;
  color: white;
  padding: 10px;
}
</style>
