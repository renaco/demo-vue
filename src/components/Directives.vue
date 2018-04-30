<template>
  <div class="directives">
    <h4>This is another component</h4>
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
      }
    }
  }
</script>
