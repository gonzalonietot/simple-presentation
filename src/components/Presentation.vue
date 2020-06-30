<template>
  <section class="container">
    <h1 class="title">Hola mi nombre es <span class="text-color-main">Gonzalo</span>,
      <br>solo soy un simple desarrollador</h1>
  </section>
</template>

<script>
  export default {
    name: 'Presentation'
  }
</script>

<style scoped>
 .container {
   width: 100%;
   padding-right: 15px;
   padding-left: 15px;
   margin-right: auto;
   margin-left: auto;
 }
 h1 {
   animation-duration: 3s;
   animation-name: slidein;
   animation-iteration-count: initial;
   animation-direction: alternate;
 }
 @keyframes slidein {
   from {
     margin-left: 100%;
     width: 100%
   }
   to {
     margin-left: 0%;
     width: 100%;
   }
 }
 .title {
   font-weight: 700;
   text-align: center;
 }
 .text-color-main {
   -webkit-text-fill-color: #00cdac;
 }
</style>