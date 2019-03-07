<template>
  <div class="hello">
    <Segment backgroundColor="1" borderStatus="1">
      <BreadCrumb>
      </BreadCrumb>
    </Segment>
    <slot></slot>
  </div>
</template>

<script>
import Segment from '../components/Segment'
import BreadCrumb from '../components/BreadCrumb'
export default {
  name: 'StatusLayout',
  components: {
    BreadCrumb,
    Segment
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
