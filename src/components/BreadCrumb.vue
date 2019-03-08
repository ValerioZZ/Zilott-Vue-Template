<template>
  <div class="hello">
    <div class="breadCrumb">
      <Segment backgroundColor="0" borderStatus="0" padding="">
        <b-container center>
          <b-row>
            <b-col xl="3" lg="12" class="personalThumb">
                <img src="../assets/valerio.png" class="img"/>
            </b-col>
            <b-col xl="9" lg="12"  class="content">
              <div class="name">Sarath Laksman</div>
              <div><img src="../assets/ActiveMail.png"/><span class="shareE">Share Profile with Hiring Manager</span></div>
              <div><img src="../assets/InActiveMail.png"/><span class="candidateE">Email Candidate(sarah@gmail.com)</span></div>
              <div><img src="../assets/phone.png"/><span class="phone">901-023-876</span></div>
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
  margin: 20px;
  padding: 10px;
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
  color: black;
  font-weight: 800;
}

.candidateE {
  color: #929395;
  font-size: 20px;
  word-wrap: break-word;
}

.shareE {
  color: #129df6;
  font-size: 20px;
}

.phone {
  color: black;
  font-size: 20px;
}
</style>
