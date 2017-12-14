<template>
  <div class="baseComponent">
    <h1>
      Im am the base component
    </h1>
  </div>
</template>

<script>
export default {
  name: 'baseComponent',
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
    warning1 () {
      console.log('Im the base component warn 1')
    },
    warning2 () {
      console.log('Im the base component warn 2')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .baseComponent {
    outline: 1px solid red;
    margin: 15px;
  }
</style>
