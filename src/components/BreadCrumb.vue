<template>
  <div class="hello">
    <div class="breadCrumb">
      <Segment backgroundColor="0" borderStatus="0">
        <b-container fluid class="">
          <b-row>
            <b-col>
              <img src="../assets/valerio.png" class="personalThumb"/>
            </b-col>
            <b-col>
              <p>Sarath Laksman</p>
              <p>Sarath Laksman</p>
              <p>Sarath Laksman</p>
            </b-col>
          </b-row>
        </b-container>
      </Segment>
    </div>
  </div>
</template>

<script>
import Segment from './Segment'
export default {
  name: 'BreadCrumb',
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

.breadCrumb {
  max-width: 600px;
}
.personalThumb {
  border-radius: 50%;
  max-width: 100px;
  max-height: 100px;
}
</style>
