<template>
  <div class="navbar">
    <h1>YO SOY UN NAVBAR</h1>
    <!-- INTARATION 3: BONUS  -->
    <button @click="helloWord"> Decir Hola!</button>
  </div>
</template>

<script>
export default {
  methods:{
    helloWord(){
      console.log("Hola!!");
    }
  }
}

</script>

<style>
.navbar{
  background-color: aquamarine;
  color: blue;
  padding: 20px;
}
</style>
