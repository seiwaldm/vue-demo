<template>
  <h1>Actions / Events</h1>
  <h2>Click-Event</h2>
  <button v-on:click="sayHello">Klick mich!</button>
  <button @click="sayHello">Klick mich!</button>

  <h2>Mousover-Event</h2>
  <img
    v-bind:src="image"
    @mouseover="changeImage"
    @mouseleave="changeImageBack"
    alt="Some Image"
  />
</template>

<script>
export default {
  data: function() {
    return {
      image: require("@/assets/meme1.jpg"),
    };
  },
  methods: {
    sayHello: function() {
      alert("Hey you!");
    },
    changeImage() {
      this.image = require("@/assets/meme2.jpg");
    },
    changeImageBack() {
      this.image = require("@/assets/meme1.jpg");
    },
  },
};
</script>
