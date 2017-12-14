<template>
  <div class="childSelects">
    <select name="" id="">
      <option value="">childSelects 1</option>
      <option value="">childSelects 2</option>
    </select>
    <select name="" id="">
      <option value="">childSelects 3</option>
      <option value="">childSelects 4</option>
    </select>
    <button @click="remove()">
      remove item child
    </button>
  </div>
</template>

<script>
export default {
  name: 'childSelects',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    remove () {
      this.$emit('remove')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
