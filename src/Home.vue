<template>
  <v-ons-page>
    <p style="text-align: center">
      Counter
    </p>
    <div id="vue-counter">
  <h3>Counter: {{ counter }}</h3>
    <button type="button" v-on:click="increase">Increase By 1</button> <button type="button" v-on:click="decrease">Decrease By 1</button> <button type="button" v-on:click="reset">Reset Counter</button>
  </div>
  </v-ons-page>
</template>

<script>
export default {
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increase: function() {
      this.counter++;
    },
    decrease:  function() {
      this.counter--;
    },
    reset: function() {
      this.counter = 0;
    }
  },
};
</script>
