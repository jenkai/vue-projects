<template>
  <div class="center">
    <button @click="click">click me</button>
    <div class="popup" v-bind:class="{ '-show': show }">
      <button class="popup-close" @click="click">close</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Popup",
  data() {
    return {
      show: false,
    };
  },
  methods: {
    click() {
      this.show = !this.show;
    },
  },
};
</script>

<style scoped>
.center {
  display: flex;
  align-items: center;
  justify-content: center;

  width: 100vw;
  height: 100vh;
}
.popup {
  display: none;
  position: fixed;
  width: 700px;
  height: 500px;
  opacity: 1;
  border-radius: 10px;
  background-color: gray;
  z-index: 1;
}

.popup.-show {
  display: flex;
  align-items: flex-start;
  justify-content: flex-end;
}

.popup-close {
}
</style>
