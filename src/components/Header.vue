<template>
  <div class="container">
    <div><h3>Vue js</h3></div>
    <div class="list">
      <nav>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
      </nav>
    </div>
  </div>
</template>
<script>
export default {
  name: 'Header',
};
</script>
<style scoped>
*{
    margin:0;
    border: 0;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
}
.container {
  display: flex;
  justify-content: space-between;
}
.container .list nav {
  display: flex;
  justify-content: space-around;
}
.container li {
list-style: none;
border:2px;
padding:4px;
margin: 4px;
}

</style>
