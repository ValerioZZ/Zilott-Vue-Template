<template>
  <div class="SubHeader">
    <b-container fluid>
      <b-row>
        <b-col sm="6"><div class="profileTitle">Full Profile</div></b-col>
        <b-col sm="6"><div class="statusTitle">Status and Notes</div></b-col>
      </b-row>
      <b-row>
        <b-col sm="3" ></b-col>
        <b-col sm="3" ></b-col>
        <b-col sm="3" class="border"></b-col>
        <b-col sm="3"></b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'SubHeader',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.SubHeader {
  margin-top: 20px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  font-size: 20px;
  border-bottom: 1px solid #d9d9d9;
}

.profileTitle {
  margin-right: 10px;
  text-align: right;
  font-weight: 800;
  color: #909193;
}

.statusTitle {
  margin-left: 10px;
  margin-bottom: 20px;
  text-align: left;
  font-weight: 800;
}

.border {
  border-bottom: 1px solid black !important;
}
</style>
