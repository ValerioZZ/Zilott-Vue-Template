<template>
  <div class="NoteSalary">
    <Segment backgroundColor="1" borderStatus="0" padding="">
      <b-container center>
        <b-row>
          <b-col sm="2" class="personalThumb">
              <img src="../../assets/valerio.png" class="img"/>
          </b-col>
          <b-col sm="10" class="content">
            <div class="name">Sarath Laksman</div>
          </b-col>
        </b-row>
      </b-container>
    </Segment>
  </div>
</template>

<script>
import Segment from '../Segment'

export default {
  name: 'NoteSalary',
  components: {
    Segment
  },
  data () {
    return {
      backgroundColor: ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.NoteSalary {
  width: 100%;
  margin: 20px 20px 0 20px;
  padding: 10px 10px 0px 10px;
}

.personalThumb {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.img {
  border-radius: 50%;
  max-width: 50px;
  max-height: 50px;
  margin: 10px 0;
  filter: blur(2px);
}

.content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: left;
  margin-bottom: 10px;
}

.name {
  margin-left: 10px;
  font-size: 18px;
  color: black;
  font-weight: 800;
}
</style>
