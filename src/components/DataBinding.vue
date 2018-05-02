<template>
  <div>
    <h1>{{ titleMessage }}</h1>
    <input type="text" v-model="messageReady" />
    <p>{{ messageReady }}</p>
  </div>
</template>

<script>
  export default {
    name: 'DataBinding',
    props: {
      message: String
    },
    data: () => {
      return {
        messageReady: 'some things',
        titleMessage: 'Title default'
      }
    }
  }
</script>

<style>
  h1 {
    font-size: 2.5em;
    color:cadetblue;
  }
</style>
