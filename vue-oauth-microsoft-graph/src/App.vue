<template>
  <div>
    <home-page class="homepage"></home-page>
  </div>
</template>

<script>
  import HomePage from './components/HomePage.vue'

export default {
  name: 'App',
  components: {
    HomePage
  }
}
</script>

<style>
.homepage{
  text-align: center;
}
</style>
