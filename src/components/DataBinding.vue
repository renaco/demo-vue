<template>
  <div>
    <h1>{{ message }}</h1>
    <input type="text">
  </div>
</template>

<script>
  export default {
    name: 'DataBinding',
    props: {
      message: String
    }
  }
</script>

<style>
  h1 {
    font-size: 2.5em;
    color:cadetblue;
  }
</style>
