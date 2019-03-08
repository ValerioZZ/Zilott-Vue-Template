<template>
  <div class="NotePresent">
    <Segment backgroundColor="1" borderStatus="0" padding="">
      <b-container center>
        <b-row>
          <b-col sm="2" class="personalThumb">
              <img src="../../assets/valerio.png" class="img"/>
          </b-col>
          <b-col sm="10" class="content">
            <div class="name">"Had a good presentation skills but his final answer  was a terrible solution"</div>
            <div class="skills">
              <div class="skillItem">Friendly</div>
              <div class="skillItem">Not Responsive</div>
            </div>
            <div class="tag">Hiring Manager  26 Dec, 2017</div>
          </b-col>
        </b-row>
      </b-container>
    </Segment>
  </div>
</template>

<script>
import Segment from '../Segment'

export default {
  name: 'NotePresent',
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

.NotePresent {
  width: 100%;
  margin: 0 20px 10px 20px;
  padding: 10px 10px 0px 10px;
}

.personalThumb {
  margin-top: 10px;
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
  margin-top: 10px;
  margin-bottom: 10px;
}

.name {
  margin-left: 10px;
  font-size: 18px;
  color: black;
  font-weight: 800;
}

.skills {

}
.skillItem {
  background-color: #cbced3;
  border-radius: 30px;
  display: inline-block;
  padding: 10px 15px 10px 15px;
}

.tag {
  margin-left: 10px;
  font-size: 18px;
  font-weight: 800;
  color: #949597
}
</style>
