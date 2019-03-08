<template>
  <div class="hello">
    <div class="Note">
      <Segment backgroundColor="0" borderStatus="0" padding="">
        <b-container center>
          <b-row>Notes</b-row>
          <b-row>
            <NoteSalary />
          </b-row>
          <b-row>
            <NoteSkill />
          </b-row>
          <b-row>
            <NotePresent />
          </b-row>
          <b-row>
            <NoteSelectSkills />
          </b-row>
        </b-container>
      </Segment>
    </div>
  </div>
</template>

<script>
import Segment from '../Segment'
import NoteSalary from './NoteSalary'
import NoteSkill from './NoteSkill'
import NotePresent from './NotePresent'
import NoteSelectSkills from './NoteSelectSkills'
export default {
  name: 'Note',
  components: {
    Segment,
    NoteSalary,
    NoteSkill,
    NotePresent,
    NoteSelectSkills
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

.Note {
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
  margin-top: 30px;
  margin-bottom: 10px;
}

.name {
  margin-left: 10px;
  font-size: 20px;
  color: black;
  font-weight: 800;
}

</style>
