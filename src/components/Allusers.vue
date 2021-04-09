<template>
<div>
    <ul>
        <li>
            <b>Name-</b>
            <b>Branch</b>
        </li>
        <li v-for="(name,index) of users" :key="index" >
            {{name.name}}-{{name.branch}}
        </li>
    </ul>
</div>
</template>
<script>
export default {
  name: 'Allusers',
  mounted() {
    this.loadData();
  },
  data() {
    return {
      users: [
        { name: 'ravi', branch: 'CSE' },
        { name: 'teja', branch: 'IT' },
        { name: 'sai', branch: 'ECE' },
      ],
    };
  },
  methods: {
    loadData() {
      this.users.push({ name: 'prabhas', branch: 'Civil' }, { name: 'storm', branch: 'mech' });
    },
  },
};
</script>
<style scoped>
*{
    list-style: none;
}
div li{
    border:10px;
    font-family: cursive;
}
</style>
