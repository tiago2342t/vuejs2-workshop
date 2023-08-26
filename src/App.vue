<template>
  <div id="app">
    <HeaderNavbar/>
    <JobCards/>
  </div>
</template>

<script>
import HeaderNavbar from './components/HeaderNavbar.vue';
import JobCards from './components/JobCards.vue';

export default {
  name: 'App',
  components: {
    HeaderNavbar,
    JobCards
  }
}
</script>

<style></style>
