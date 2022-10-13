<template>
  <div>
    <HomePage></HomePage>
  </div>
</template>

<script>
import KeyPanel from './components/KeyPanel.vue';
import HomePage from './components/HomePage.vue';

export default {
  name: 'App',
  components: {
    KeyPanel,
    HomePage,
}
}
</script>
