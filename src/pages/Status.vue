<template>
  <div class="hello">
    <Segment backgroundColor="0" borderStatus="1">
      <p class="companyTitle">ZILOTT</p>
      <b-container fluid>
        <b-row>
          <b-col xl="1" lg="12" offset-xl="1"><ArrowLeftThumb /></b-col>
          <b-col xl="7" lg="12"><StatusLayout /></b-col>
          <b-col xl="2" lg="12"><SocialDetail /></b-col>
        </b-row>
      </b-container>
    </Segment>
  </div>
</template>

<script>
import Segment from '../components/Segment'
import StatusLayout from '../layouts/StatusLayout'
import ArrowLeftThumb from '../components/ArrowLeftThumb'
import SocialDetail from '../components/SocialDetail'
export default {
  name: 'Status',
  components: {
    StatusLayout,
    Segment,
    ArrowLeftThumb,
    SocialDetail
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
.companyTitle {
  margin-top: 20px;
  font-size: 40px;
  font-weight: 900;
}

.content {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
</style>
