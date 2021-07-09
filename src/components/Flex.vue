<template>
  <div class="row">
    <div class="box1">
      <div>this is box 1</div>
      <div></div>
      <div></div>
    </div>
    <div class="box2">this is box 2</div>
    <div class="box3">this is box 3</div>
    <div class="box4">
      <div>box-1</div>
      <div>box-1</div>
    </div>
    <div class="box1">this is box 1</div>
    <div class="box5">this is box 5</div>
    <div class="box1">this is box 1</div>
    <div class="box4">this is box 4</div>
    <div class="box5">this is box 5</div>
    <div class="box1">this is box 1</div>
    <div class="box1">this is box 1</div>
    <div class="box6">this is box 6</div>
    <div class="box2">this is box 2</div>
    <div class="box4">this is box 4</div>
    <div class="box5">this is box 5</div>
    <div class="box2">this is box 2</div>
    <div class="box6">this is box 6</div>
  </div>
</template>

<style scoped>
.row {
  display: flex;
  justify-content: flex-start;

  align-items: stretch;
  align-content: space-between;
  flex-flow: wrap;
}

.box2 {
  background-color: cadetblue;
  height: 60vh;
  margin: 10px;
  flex: 3;
}

.box3 {
  background-color: cadetblue;
  height: 50vh;
  margin: 10px;
  flex: 4;
}
.box4 {
  background-color: cadetblue;
  height: 40vh;
  margin: 10px;
  flex-basis: 20vw;
  display: flex;
  justify-content: space-evenly;
}
.box4 > div {
  background-color: khaki;
  display: flex;
  align-items: center;
}

.box5 {
  background-color: cadetblue;
  white-space: pre;
  height: 30vh;
  margin: 10px;
  flex-basis: 20vw;
}
.box6 {
  background-color: cadetblue;
  height: 20vh;
  margin: 10px;
  flex-basis: 20vw;
}
.box1 {
  display: flex;
  background-color: cadetblue;
  align-items: stretch;
  margin: 10px;
  flex: 2;
  justify-content: space-evenly;
  flex-flow: column;
  min-width: 150px;
}
.box1 > div {
  width: 100%;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: khaki;
}
</style>
