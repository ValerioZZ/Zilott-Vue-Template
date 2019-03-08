<template>
  <div class="NoteSelectSkills">
    <Segment backgroundColor="0" borderStatus="0" padding="">
      <b-container center>
        <b-row>
          <b-col sm="12" class="content">
            <div><textarea class="skillInput"></textarea> </div>
            <div class="skills">
              <div class="tagItem">Add Tags:</div>
              <div class="skillItem">Friendly</div>
              <div class="skillItem">Not Responsive</div>
              <div  class="skillItem" v-for="(item, index) in items">
                  {{ item }}
              </div>
            </div>
          </b-col>
        </b-row>
        <b-row><b-button variant="primary">Submit</b-button></b-row>
      </b-container>
    </Segment>
  </div>
</template>

<script>
import Segment from '../Segment'

export default {
  name: 'NoteSelectSkills',
  components: {
    Segment
  },
  data () {
    return {
      backgroundColor: '',
      items: ['Friendly', 'PLEASANT TO INTERACT', 'RESPONSIVE', 'UNPROFESSIONAL', 'DIDNT SHOW FOR INTERVIEW', 'LATE FOR INTERVIEW','FREQUENT RESCEDULING', 'RUDE']
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.NoteSelectSkills {
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

.skillInput {
  width: 100%;
  height: 200px;
  padding: 12px 20px;
  margin: 8px 0;
  box-sizing: border-box;
  border-radius: 10px;
  border-width: 2px;
  border-color: #129df6;
  background-color: white;
}

.skills {

}
.tagItem {
  background-color: #f2f3f5;
  border-radius: 30px;
  display: inline-block;
  padding: 10px 15px 10px 15px;
  color: black;
  font-size: 20px;
  font-weight: 600;
}
.skillItem {
  background-color: #cbced3;
  border-radius: 30px;
  display: inline-block;
  padding: 10px 15px 10px 15px;
  margin-right: 3px;
  margin-bottom: 5px;
}
</style>
