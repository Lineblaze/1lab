<template>
  <header>
    <div class="logo"><img src="../assets/logo.png" width=40></div>
    <nav>
      <p><router-link to="/">Главная</router-link></p>
      <p><router-link to="/news">Новости</router-link></p>
    </nav>
  </header>
</template>

<script>

export default {
  name: 'Header'
}
</script>

<style scoped>
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 7px 20px;
  }
  
  nav {
    display: flex;
  }
  
  p {
    margin-right: 25px;
  }
  
  p:last-child {
    margin-right: 0;
  }
</style>