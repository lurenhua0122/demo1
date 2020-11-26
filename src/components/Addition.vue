<template>
  <div >
      <h3>当前最新的COUNT值为：{{this.$store.state.count}}</h3>
      <button type="button" @click="add">+1</button>
      <button type="button" @click="add2(3)">+N</button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data () {
    return {}
  },
  methods: {
    add () {
      this.$store.commit('add')
    },
    add2 (n) {
      this.$store.commit('add2', 3)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
