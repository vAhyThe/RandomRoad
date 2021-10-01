<template>
  <div>
    <button @click="randomForward()" class="btn btn-primary">Levo</button>
    Pujdeš <span>{{ randomForwardValue }}</span>
    <div>
      <h2>Počet levo</h2>
      <input type="range" name="vol" min="1" max="50" v-model="rangeValue">
      <div>
        {{ rangeValue }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "left",

  data() {
    return {
      randomForwardValue: 10,
      rangeValue: 10,
    }
  },

  methods: {
    randomForward() {
      this.randomForwardValue = (Math.floor(Math.random() * this.rangeValue) + 1);
    },
  },
};
</script>
