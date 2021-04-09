<template>
  <div class="container">

    <header><b>Dashboard</b></header>
    <nav>
      <li><router-link to="/allusers">All users</router-link></li>
      <li><router-link to="/Mydetails">mydetails</router-link></li>
    </nav>
  </div>
</template>
<script>
/* eslint-disable eol-last */
export default ({
  name: 'Sidenav',
});
</script>
<style scoped>
*{
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
    list-style: none;
    text-decoration: none;
}
.container{
    display: flex;
    position: relative;
    width:200px;
    height: 100%;
    position: fixed;
    flex-direction: column;
}
.container header{
    position: relative;
    right: 60px;
    font-style: initial;
    font-family: cursive;
    font-size: medium;
    padding: 30px;
}
.container li{
    list-style: none;
    padding: 30px;
    position: relative;
    right: 60px;
}
</style>