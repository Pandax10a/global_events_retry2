<template>
  <div id="app">
   <user-lists></user-lists>
   <special-user></special-user>
   <h1> this is app vue</h1>
  </div>
</template>

<script>
import UserLists from '@/components/UserLists.vue';
import SpecialUser from '@/components/SpecialUser.vue';

export default {
  name: 'app',
  components: {
    UserLists,
    SpecialUser
  },
};


</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
