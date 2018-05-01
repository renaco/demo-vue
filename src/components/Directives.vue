<template>
  <div class="directives">
    <h4>This is another component {{ dataToShow }}</h4>
    <section v-if="conected"> This is my section </section>
    <button v-on:click="showSection">Show section</button>
  </div>
</template>

<script>
  export default {
    name: 'Directives',
    methods: {
      showSection: function() {
        this.conected = true;
        this.dataToShow = 'Some title',
        console.log('click', this.conected ? true: false)
      },
    },
    data: () => {
      return {
        conected: false,
        dataToShow: '...'
      }
    }
  }
</script>

<style>
  button {
    padding: 5px 15px;
  }
  section {
    padding: 20px;
    font-size: 2em;
  }
</style>
