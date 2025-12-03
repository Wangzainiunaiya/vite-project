<template>
 <div>
  <h1>My Header</h1>
  <nav>
   <ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Contact</a></li>
    <li><a href="#">Contact</a></li>
    <li><a href="#">Contact</a></li>
   </ul>
  </nav>
 </div> 
</template>

<script setup lang='ts'>
 
</script>

<style scoped>
  h1 {
    color: #333;
  }
  nav ul {
    list-style-type: none;
    padding: 0;
  }
  nav ul li {
    display: inline;
    margin-right: 15px;
  }
  nav ul li a {
    text-decoration: none;
    color: #007BFF;
  }
  nav ul li a:hover {
    text-decoration: underline;
  }
</style>