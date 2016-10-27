
<template>
  <div id="app">
    <h1><%= name %></h1>
    <p><%= description %></p>

    <router-view class="view" />
  </div>
</template>

<style>
  body {
    font-family: Verdana, sans-serif;
  }
</style>

<script>
  import Home from './home';
  import About from './about';

  export default {
    name: 'container',
    components: {
      home: Home,
      about: About
    }
  };
</script>
