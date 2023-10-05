<script>
 export default {
    name: "Navbar",
 };
</script>

<template>
  <nav>
    <ul class="nav_bar_first">
      <li><a href="#">abbbrr</a></li>
    </ul>
    <ul class="nav_bar_second">
      <li><a href="#">About me</a></li>
      <li><a href="#">Services</a></li>
      <li><a href="#">Contact me</a></li>
    </ul>
  </nav>
</template>

<style>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap');

  nav {
    color: #fff;
    display: flex;
    justify-content: space-between;
    margin: 30px
  }

  ul {
    list-style-type: none;
    padding: 0;
  }
  .nav_bar_first li a {
    text-decoration: none;
    color: #FFF;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 33px;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
  }
  .nav_bar_second li a {
    text-decoration: none;
    color: #FFF;
    font-family: 'Open Sans', sans-serif;
    font-size: 18px;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
  }
  .nav_bar_second {
    display: flex;
    justify-content: space-around;
  }
  .nav_bar_second li {
    margin: 20px;
  }

    @media (max-width: 768px) {
    nav {
      flex-direction: column;; 
      justify-content: space-between;
      align-items: center;
    }

    .nav_bar_second {
      flex-direction: row;
    }

    .nav_bar_second li {
      margin: 10px; 
    }
  }
</style>