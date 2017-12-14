<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <list-selects>
    </list-selects>

    <div class="test-share-template">
      <h4>
        Shared template with extend
      </h4>
      <base-component></base-component>
      <hr>
      <new-component></new-component>
    </div>

    <div>
      <h4>
        Shared template with HTML loader
      </h4>
      <shared-template-one></shared-template-one>
      <shared-template-two></shared-template-two>
    </div>
  </div>
</template>

<script>
import ListSelects from './ListSelects'
import BaseComponent from './BaseComponent'
import NewComponent from './NewComponent'
import sharedTemplateOne from './sharedTemplateOne'
import sharedTemplateTwo from './sharedTemplateTwo'

export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    ListSelects,
    BaseComponent,
    NewComponent,
    sharedTemplateOne,
    sharedTemplateTwo
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
