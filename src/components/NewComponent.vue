
<script>
import BaseComponent from './BaseComponent'

export default {
  name: 'newComponent',
  extends: BaseComponent,
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    warning2 () {
      console.log('Im override the method of base component warn 2')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .newComponent {
    outline: 1px solid blue;
    margin: 15px;
  }
</style>
