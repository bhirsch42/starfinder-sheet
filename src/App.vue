<template>
  <div id="app" class="container">
    <GeneralInfo :character="character"/>
    <div class="row">
      <div class="col-sm-6">
        <AbilityScores :character="character"/>
      </div>
      <div class="col-sm-6">
        <Initiative :character="character"/>
        <HealthAndResolve :character="character"/>
      </div>
    </div>
  </div>
</template>

<script>
import styles from '@/styles/app.scss'
import GeneralInfo from '@/components/GeneralInfo'
import AbilityScores from '@/components/AbilityScores'
import Initiative from '@/components/Initiative'
import HealthAndResolve from '@/components/HealthAndResolve'

export default {
  name: 'App',
  components: {
    GeneralInfo,
    AbilityScores,
    Initiative,
    HealthAndResolve
  },
  data() {
    return {
      character: {
        name: 'Evdokayo',
        abilityScores: [
          { name: 'Strength', score: 10, upgradedScore: null },
          { name: 'Dexterity', score: 10, upgradedScore: null },
          { name: 'Constitution', score: 10, upgradedScore: null },
          { name: 'Intelligence', score: 10, upgradedScore: null },
          { name: 'Wisdom', score: 10, upgradedScore: null },
          { name: 'Charisma', score: 10, upgradedScore: null },
        ],
        health: {
          staminaPoints: {
            total: 0,
            current: 0,
          },
          hitPoints: {
            total: 0,
            current: 0,
          },
          resolvePoints: {
            total: 0,
            current: 0,
          },
        }
      }
    }
  }
}
</script>

<style lang="scss">
</style>
