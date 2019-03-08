<template>
  <div :class="background" :style="border ? borderStyle : ''">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'Segment',
  props: ['backgroundColor', 'borderStatus'],
  data () {
    return {
      msg: 'Welcome to Your Vue.js App',
      background: this.backgroundColor === '0' ? 'segmentGrey' : 'segmentDark',
      borderStyle: {
        'border': '2px solid #d9d9d9'
      },
      border: this.borderStatus === '1' ? 1 : 0
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

.segment {
  background-color: #f2f3f5;
  border: 1px solid #d9d9d9;
}
.segmentGrey {
  background-color: #f2f3f5;
  border-radius: 5px;
}

.segmentDark {
  background-color: white;
  border-radius: 5px;
}

</style>
