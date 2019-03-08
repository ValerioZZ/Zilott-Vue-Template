<template>
  <div class="SocialDetail">
    <Segment backgroundColor="1" borderStatus="1" padding="">
      <div>
        <div class="block">
          <img src="../assets/InActiveMail.png" class="img" />
          <span class="name">Email Candidate</span>
        </div>
        <div class="block">
          <img src="../assets/InActiveMail.png" class="img" />
          <span class="name">Share Profile</span>
        </div>
      </div>
      <div>
        <div class="item">LinkedIn</div>
        <div class="item">StackOverflow</div>
        <div class="item">Github</div>
        <div class="item">Blog / Website</div>
      </div>
    </Segment>
  </div>
</template>

<script>
import Segment from './Segment'
export default {
  name: 'SocialDetail',
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

.SocialDetail {
  margin: 10px 20px 20px 20px;
  padding: 10px 10px 10px 10px;
  width: 100%;
}

.block {
  text-align: left;
  padding-left: 10px;
  margin: 30px 0;
  padding-bottom: 30px;
  border-bottom: 2px solid #d9d9d9;
}

.content {
  padding-top: 20px;
}

.title {
  color: black;
  font-weight: 900;
  font-size: 20px;
}
.personalThumb {
  margin-top: 30px;
}

.img {
  max-width: 110px;
  max-height: 110px;
}
.name {
  margin-left: 5px;
  margin-top: 15px;
  font-size: 20px;
  color: black;
  font-weight: 800;
}

.item {
  text-align: left;
  margin-left: 15px;
  margin-bottom: 20px;
  font-size: 18px;
  font-weight: 800;
  color: #949597
}

</style>
