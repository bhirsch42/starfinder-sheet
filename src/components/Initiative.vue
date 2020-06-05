<template>
  <div class="card">
    <div class="card-title">Initiative</div>
    <div class="card-body d-flex">
      <div class="input-group">
        <label>Total</label>
        <input type="number">
      </div>
      <div class="math-symbol">=</div>
      <div class="input-group">
        <label>Dex Modifier</label>
        <input type="number">
      </div>
      <div class="math-symbol">+</div>
      <div class="input-group">
        <label>Misc Modifier</label>
        <input type="number">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Initiative',
  props: ['character']
}
</script>
