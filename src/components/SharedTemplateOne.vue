<template src="./mySharedTemplate.html"></template>

<script>
export default {
  name: 'sharedTemplateOne',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  mounted () {
    this.warning1()
    this.warning2()
  },
  methods: {
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .sharedTemplateOne {
    outline: 1px solid red;
    margin: 15px;
  }
</style>
