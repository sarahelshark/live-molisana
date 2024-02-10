<script>
export default {
  name: "AppHeader",
};
</script>

<template>
  <header>
    <div class="logo">
      <img src="/img/la-molisana-logo.png" alt="" />
    </div>

    <nav>
      <ul class="main_menu">
        <li><a href="#">Home</a></li>
        <li><a href="#">Prodotti</a></li>
        <li><a href="#">chi siamo</a></li>
        <li><a href="#">Contatti</a></li>
      </ul>
    </nav>
  </header>
</template>

<style scoped >
header {
  text-align: center;
  & .main_menu {
    list-style: none;
    display: flex;
    justify-content: center;

    & a {
      text-decoration: none;
      padding: 0.5rem 1rem;
      color: #333;
    }
  }
}
</style>
