<template>
  <div class="card">
    <div class="card-title">
      Health and Resolve
    </div>
    <div class="card-body">
      <table>
        <tr>
          <th></th>
          <th>Stamina Points</th>
          <th>Hit Points</th>
          <th>Resolve Points</th>
        </tr>
        <tr>
          <td>Total</td>
          <td>
            <input type="number" v-model="character.health.staminaPoints.total">
          </td>
          <td>
            <input type="number" v-model="character.health.hitPoints.total">
          </td>
          <td>
            <input type="number" v-model="character.health.resolvePoints.total">
          </td>
        </tr>
        <tr>
          <td>Current</td>
          <td>
            <input type="number"
                   v-model="character.health.staminaPoints.current"
                   :min="0"
                   :max="character.health.staminaPoints.total">
          </td>
          <td>
            <input type="number"
                   v-model="character.health.hitPoints.current"
                   :min="0"
                   :max="character.health.hitPoints.total">
          </td>
          <td>
            <input type="number"
                   v-model="character.health.resolvePoints.current"
                   :min="0"
                   :max="character.health.resolvePoints.total">
          </td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HealthAndResolve',
  props: ['character'],
}
</script>
