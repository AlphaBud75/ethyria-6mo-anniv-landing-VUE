<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>

  <div class='SectionPortals'>
    <SectionPortals />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import SectionPortals from '@/components/portals.vue';

export default {
  name: 'HomeView',
  components: {
    HelloWorld,
    SectionPortals,
  },
};
</script>
