<template>
  <div class="card">
    <div class="card-title">General Info</div>
    <div class="card-body">
      <div class="row">
        <div class="col-sm-7">
          <div class="input-group">
            <label>Character Name</label>
            <input type="text" v-model="character.name">
          </div>
          <div class="d-flex">
            <div class="input-group">
              <label>Class / Level</label>
              <input type="text" v-model="character.class">
            </div>
            <div class="input-group">
              <label>Race</label>
              <input type="text" v-model="character.race">
            </div>
            <div class="input-group">
              <label>Theme</label>
              <input type="text" v-model="character.name">
            </div>
          </div>
          <div class="d-flex">
            <div class="input-group">
              <label>Size</label>
              <input type="text" v-model="character.size">
            </div>
            <div class="input-group">
              <label>Speed</label>
              <input type="text" v-model="character.speed">
            </div>
            <div class="input-group">
              <label>Gender</label>
              <input type="text" v-model="character.gender">
            </div>
            <div class="input-group">
              <label>Home World</label>
              <input type="text" v-model="character.homeWorld">
            </div>
          </div>
          <div class="d-flex">
            <div class="input-group">
              <label>Alignment</label>
              <input type="text" v-model="character.alignment">
            </div>
            <div class="input-group">
              <label>Deity</label>
              <input type="text" v-model="character.deity">
            </div>
            <div class="input-group">
              <label>Player</label>
              <input type="text" v-model="character.player">
            </div>
          </div>
        </div>
        <div class="col-sm-5">
          <div class="input-group">
            <label>Description</label>
            <textarea v-model="description"></textarea>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'GeneralInfo',
  props: ['character']
}

</script>
