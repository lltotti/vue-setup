<template>
  <div :id="myClass">
    <!-- INTERATION 1 -->
    <Navbar />
   <!-- INTERATION 2 -->
    <h2>Ahora en Barcelona: {{ date}}</h2>
       
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
export default {
  components:{
    Navbar
  },
  data() {
    const d = new Date();
     return {
      date: d.getHours()+":"+d.getMinutes()+":"+d.getSeconds(),
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
