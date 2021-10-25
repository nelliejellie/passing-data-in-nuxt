<template>
  <div>
    <ListOne />
    <nuxt-link to="/pagetwo" class="button">Next</nuxt-link>
  </div>
  
</template>

<script>
export default {

}
</script>

<style scoped>
  div{
    height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: center;
    width: 100vw;
  }
  .button{
    text-align: center;
    color: white;
    background: black;
    width: 10vw;
    padding: 20px 0px;
    border-radius: 10px;
  }
</style>
