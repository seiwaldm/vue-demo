<template>
  <h1>Expressions</h1>
  <p>I have a {{ animal.pic }}</p>
  <p>He is... {{ isCute ? "sweet!" : "ugh!" }}</p>
  <p>{{ animal.name }} says {{ animal.makeNoise() }}</p>
</template>

<script>
export default {
  data: function() {
    return {
      animal: {
        name: "Porky",
        pic: "🐷",
        makeNoise: function() {
          return "Oink!";
        },
      },
      isCute: false,
    };
  },
};
</script>
