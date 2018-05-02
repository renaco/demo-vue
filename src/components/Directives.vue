<template>
  <div class="directives">
    <h4>This is another component {{ dataToShow }}</h4>
    <section v-if="conected"> This is my section </section>
    <button v-on:click="showSection" v-if="disconected">Show section</button>
    <button v-on:click="hideSection" v-if="conected">Hide section</button>
  </div>
</template>

<script>
  export default {
    name: 'Directives',
    methods: {
      showSection: function() {
        this.conected = true;
        this.disconected = false;
        this.dataToShow = 'Some title';
        console.log('click', this.conected ? true: false)
      },
      hideSection: function() {
        this.conected = false;
        this.disconected = true;
        this.dataToShow = 'Hide element';
        console.log('click disabled', this.conected ? true: false)
      }
    },
    data () {
      return {
        disconected: true,
        conected: false,
        dataToShow: '...'
      }
    }
  }
</script>

<style>
  button {
    background: #000;
    color: white;
    padding: 5px 15px;
  }
  section {
    padding: 20px;
    font-size: 2em;
  }
</style>
