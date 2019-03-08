<template>
  <div class="statusLayout">
    <Segment backgroundColor="1" borderStatus="1">
      <SubHeader />
      <b-container>
          <b-row>
            <b-col xl="7" lg="12">
              <BreadCrumb>
              </BreadCrumb>
              <Note />
            </b-col>
            <b-col xl="5" lg="12">
              <StatusHistory />
            </b-col>
          </b-row>
      </b-container>
    </Segment>
    <slot></slot>
  </div>
</template>

<script>
import Segment from '../components/Segment'
import BreadCrumb from '../components/BreadCrumb'
import ArrowLeftThumb from '../components/ArrowLeftThumb'
import SubHeader from '../components/header/SubHeader'
import Note from '../components/Note/index'
import StatusHistory from '../components/StatusHistory'
import SocialDetail from '../components/SocialDetail'
export default {
  name: 'StatusLayout',
  components: {
    BreadCrumb,
    Segment,
    SubHeader,
    Note,
    StatusHistory,
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
.statusLayout {
  margin: 20px;
}
</style>
