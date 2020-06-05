<template>
  <div class="card">
    <div class="card-title">Ability Scores</div>
    <div class="card-body">
      <table>
        <tr>
          <th></th>
          <th>Score</th>
          <th>Modifier</th>
          <th>Upgraded<br>Score</th>
          <th>Upgraded<br>Modifier</th>
        </tr>
        <tr v-for="abilityScore in character.abilityScores">
          <td>
            {{ abilityScore.name }}
          </td>
          <td>
            <input type="number" v-model="abilityScore.score">
          </td>
          <td>
            <input type="number" disabled :value="Math.floor((abilityScore.score - 10) / 2)">
          </td>
          <td>
            <input type="number" v-model="abilityScore.upgradedScore">
          </td>
          <td>
            <input type="number" disabled :value="Math.floor((abilityScore.upgradedScore - 10) / 2)">
          </td>
        </tr>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: 'AbilityScores',
  props: ['character']
}
</script>
