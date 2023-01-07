<script setup></script>

<template>
  <div id="game">
    <section class="row">
      <div class="col-6 character">
        <h1>You</h1>
        <div class="life-bar">
          <div class="life"><div class="percentage">100</div></div>
        </div>
      </div>
      <div class="col-6 character">
        <h1>Monster</h1>
        <div class="life-bar">
          <div class="life"><div class="percentage">100</div></div>
        </div>
      </div>
      <div class="col-12 d-flex justify-content-center actions">
        <button class="btn btn-primary">Démarrer une partie</button>
        <button class="btn btn-danger">Attack</button>
        <button class="btn btn-warning">Wildcard</button>
        <button class="btn btn-success">Heal</button>
        <button class="btn btn-secondary">Give up</button>
      </div>

      <div class="col-6 offset-3">
        <ul class="list-group col-12">
          <li class="list-group-item">Dapibus ac facilisis in</li>
          <li class="list-group-item list-group-item-danger">
            A simple danger list group item
          </li>
        </ul>
      </div>
    </section>
  </div>
</template>

<style>
.character {
  text-align: center;
}
.life-bar {
  background: grey;
  width: 200px;
  height: 25px;
  position: relative;
  margin: 0 auto;
}

.life {
  width: 200px;
  height: 25px;
  background: #29cf1b;
  position: absolute;
  left: 0;
  top: 0;
  z-index: 9;
}
.percentage {
  position: relative;
  z-index: 99;
  display: block;
  text-align: center;
  color: white;
}

.actions {
  margin: 40px auto;
}
</style>
