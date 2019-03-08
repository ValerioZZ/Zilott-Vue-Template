<template>
  <div class="StatusHistory">
    <Segment backgroundColor="0" borderStatus="0" padding="">
      <div class="section">
        <div class="decorate"></div>
        <div class="content">
          <p class="title">
            STATUS HISTORY
          </p>
          <div>
            <b-button-group>
              <b-dropdown right split text="Rejected" variant="danger">
                <b-dropdown-item>Item 1</b-dropdown-item>
                <b-dropdown-item>Item 2</b-dropdown-item>
                <b-dropdown-divider />
                <b-dropdown-item>Item 3</b-dropdown-item>
              </b-dropdown>
            </b-button-group>
          </div>
          <div class="detail">
            Tobias Funke  26 Dec, 2017, Edit
          </div>
          <div>
            <b-button>Shortliste</b-button>
          </div>
          <div class="detail">
            Tobias Funke  26 Dec, 2017, Edit
          </div>
        </div>      
      </div>
      <div class="statusList">
        <p class="title">
          STATUS HISTORY
        </p>
        <p class="normalPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="normalPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="normalPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="redPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="normalPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="redPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="normalPlus">
          +<span class="normalText">STATUS HISTORY</span>
        </p>
        <p class="inactivePlus">
          +<span class="inactiveText">STATUS HISTORY</span>
        </p>
      </div>
    </Segment>
  </div>
</template>

<script>
import Segment from './Segment'
export default {
  name: 'StatusHistory',
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

.StatusHistory {
  max-width: 600px;
  margin: 20px 20px 20px 20px;
  padding: 10px 10px 10px 10px;
}

.section {
  display: flex;
  flex-direction: row;
  border-bottom: 2px solid #d9d9d9;
}

.decorate {
  border-left: 2px solid #d9d9d9;
  border-top: 2px solid #d9d9d9;
  border-bottom: 2px solid #d9d9d9;
  height: 116px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  width:30px;
  margin-top: 90px;
  margin-left: 10px;
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
  border-radius: 50%;
  max-width: 100px;
  max-height: 100px;
}

.content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  text-align: left;
  margin-top: 30px;
  margin-bottom: 10px;
}

.name {
  margin-left: 10px;
  font-size: 20px;
  color: black;
  font-weight: 800;
}

.menuColor {
  backgroundColor: red;
}

.detail {
  margin-top: 10px;
  margin-bottom: 30px;
  margin-left: 10px;
  font-size: 18px;
  font-weight: 800;
  color: #949597
}

.statusList {
  margin-top: 30px;
  text-align: left;
  margin-left: 40px;
}

.normalPlus {
  color: green;
}

.redPlus {
  color: red;
}

.inactivePlus {
  color: #d9d9d9;
}

.normalText {
  color: black;
  margin-left: 10px;
  font-weight: 400;
}

.inactiveText {
  color: #d9d9d9;
  margin-left: 10px;
  font-weight: 400;
}
</style>
