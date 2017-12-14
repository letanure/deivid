<template>
  <div class="childSelects">
    <h1>List selects</h1>
    <div v-for="(item, index) in lista" :key="item.id">
      <div>
        <span>
          {{ item.label }}
        </span>
        <child-selects @remove="removeOnParent(index)"></child-selects>
      </div>
    </div>
    <button @click="addItem()" >
      Add item child
    </button>
  </div>
</template>

<script>
import ChildSelects from './ChildSelects'

export default {
  name: 'ListSelects',
  data () {
    return {
      lista: [],
      count: 0
    }
  },
  methods: {
    addItem () {
      this.count++
      this.lista.push({
        id: this.count,
        label: `item ${this.count}`
      })
    },
    removeOnParent (index) {
      this.$delete(this.lista, index)
    }
  },
  components: {
    ChildSelects
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
