<template>
    <div class="body row">
      <Profile></Profile>
      <Info></Info>
    </div>
  </template>
  
  <script>
  import Profile from '../components/profile.vue' 
  import Info from '../components/info.vue' 
  export default {
    name: 'IndexPage',
    components: {
      Profile,
      Info
    },
    head: {
      bodyAttrs: {
        class: 'main' // Ganti dengan kelas yang sesuai
      }
    }
  }
  </script>
  
  <style>
  .main{
    overflow-x: hidden;
    width: 100vw;
    padding: 3rem;
    height: 100vh;
  }
    .body{
      display: flex;
      height: 100%;
    }
  
  </style>
  