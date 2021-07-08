<template>
  <h1>Caculate your BMI</h1>
  <input
    v-model.lazy.number="input_height"
    type="number"
    placeholder="height(m)"
  />
  <br />
  <input
    v-model.lazy.number="input_weight"
    type="number"
    placeholder="weight(kg)"
  />
  <p>Your BMI is</p>
  <h1>{{ BMI }}</h1>
  <!-- <button @click="reset">rest</button> -->
</template>

<script>
export default {
  components: {},
  name: "Title",
  data() {
    return {
      input_height: "",
      input_weight: "",
    };
  },
  computed: {
    BMI: function() {
      if (this.input_weight > 0 && this.input_height > 0) {
        let answer =
          Math.floor(
            (this.input_weight / Math.pow(this.input_height, 2)) * 100
          ) / 100;
        return answer;
      }
      return "";
    },
  },
  methods: {
    reset() {
      this.input_height = "";
      this.input_weight = "";
    },
  },
};
</script>

<style scoped>
input {
  margin: 10px;
}
</style>
