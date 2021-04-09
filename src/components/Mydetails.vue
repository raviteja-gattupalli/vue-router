<template>
<div>
    <b>Name:</b>
    <span v-if="name.length>6">{{name}}</span>
    <span v-else>Name is less than 5</span><br>
    <b>Password:</b>
    {{password.length>10? password : "passowrd is less than 17"}}<br>
    <b>address:</b>
    <span v-if="name.length>25">{{address}}</span>
    <span v-else>Enter the address greater than 25 characters</span><br>
    <b>Phone Number:</b>
    {{phno.length==10? phno : "please enter the valid number,You entered Phone number is:"+phno}}
</div>
</template>
<script>
export default {
  name: 'Mydetails',
  data() {
    return {
      name: 'ravi Teja',
      password: 'fgjmjllortq',
      address: 'opp polocestattion',
      phno: '891999',
    };
  },
};
</script>
<style scoped>
div{
    padding:20px;
}
</style>
