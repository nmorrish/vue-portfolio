<template>
    <div class="d-flex justify-content-center name-title">
      <img alt="Nick Morrish" class="logo" src="../assets/images/profile-image.jpg" width="125" height="125" />
      <div class="name-container">
        <h1>Nick Morrish</h1>
        <h3>Full Stack Developer</h3>
      </div>
    </div>
  </template>

<script>
    export default {
        name: 'PageTitle',
        props:{
            title: String,
        },
    }
</script>

<style scoped>
  .logo{
    border-radius:50%;
    -webkit-box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
    -moz-box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
    box-shadow: 0px 0px 11px 0px rgba(0,0,0,0.75);
  }
  .name-title{
    padding-top:4rem;
    align-items: center;
    padding-bottom:3rem;
  }
  .name-container{
    margin-left:2rem;
  }

  @media(max-width:800px) {
    .name-title{
      padding-top:1rem;
      align-items: left;
      padding-bottom:0;
      flex-direction: column;
    }
    .name-container{
      margin-left:0;
      text-align: center;
    }
  }
</style>