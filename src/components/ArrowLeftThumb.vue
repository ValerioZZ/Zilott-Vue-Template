<template>
  <div class="hello">
    <div class="ArrowLeftThumb">
      <Segment backgroundColor="1" borderStatus="0" padding="">
        <div>
          <img src="../assets/arrow-left.png" class="img"/>
        </div>
        <p class="name">
          Back
        </p>
      </Segment>
    </div>
  </div>
</template>

<script>
import Segment from './Segment'
export default {
  name: 'ArrowLeftThumb',
  components: {
    Segment
  },
  data () {
    return {
      backgroundColor: '',
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.ArrowLeftThumb {
  width: 100px;
  height: 100px;
  margin: 20px;
  padding: 10px;
  border: 2px solid #d9d9d9;
  background-color: white;
  border-radius: 5px;
}

.personalThumb {
  margin-top: 30px;
}

.img {
  border-radius: 50%;
  max-width: 100px;
  max-height: 100px;
}

.content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: left;
  margin-top: 20px;
  margin-bottom: 10px;
}

.name {
  margin-left: 10px;
  font-size: 20px;
  color: #8a8a8a;
  font-weight: 800;
}
</style>
