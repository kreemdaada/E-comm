<template>
  <div>
  <HeaderView/>
  <RouterView/>
</div>
  </template>

  <script setup>
  import HeaderView from "./components/HeaderView.vue"
  </script>

  <style scoped>
 .container {
  max-width:calc(1440px - 170px);
  width:100%;
  margin:auto;
 }
 .btn{
  background:transparent;
  border:none;
  transition:.3;
  cursor:pointer;
  width:100%;
  display:flex;
  justify-content:center;
  align-items:center;
 }
 img{
  width:100%;
 }
</style>