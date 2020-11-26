<template>
  <div>
      <h3>当前最新的COUNT值为：{{count}}</h3>
      <button type="button">-1</button>
  </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data () {
    return {}
  },
  computed: {
    ...mapState(['count'])
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
