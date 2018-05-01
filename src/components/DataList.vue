<template>
  <div>
    <h4>Choose Type</h4>
    <select id="list" @change="selectItem">
      <option v-for="item in items" v-bind:value="item.value">
        {{ item.option }}
      </option>
    </select>
    <p>{{ selecteded }}</p>
    <!-- <pre>
      {{ $data }}
    </pre> -->
  </div>
</template>

<script>
export default {
  name: 'DataList',
  methods: {
    selectItem: function(e) {
      this.selecteded = e.target.value;
      console.log(e.target.value)
    }
  },
  data: () => {
    return {
        selecteded: 'wait...',
        items: [
          { option: 'Escoja', value: 0}, 
          { option: 'one', value: 1},
          { option: 'two', value: 2},
          { option: 'three', value: 3}
        ]
      }
  }
}
</script>

