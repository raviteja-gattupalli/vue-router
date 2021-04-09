<template>
  <div class="home">
    <HelloWorld msg="Welcome to Vue js" />
  </div>
</template>

<script>
import HelloWorld from '../components/HelloWorld.vue';

export default {
  name: 'Home',
  components: {
    HelloWorld,
  },
};
</script>
