<template>
  <h1>Directives</h1>
  <div>
    <h2>Vue-if</h2>
    <div v-if="product.inStock">
      {{ product.name }}
      <div v-if="product.onSale">
        🔥 OnSale!!! 🔥
      </div>
      <div v-else>💰 regular Price... 💰</div>
    </div>
  </div>
  <div>
    <h2>Vue-Model</h2>
    <input type="text" v-model.trim="inputField" />
    <p>{{ inputField }}</p>
  </div>
  <div>
    <h2>What's your age?</h2>
    <input type="number" name="" id="" v-model.number="age" />
    <div v-if="age < 16">🥤</div>
    <div v-else-if="age < 18">🥤, 🍺 &amp; 🍷</div>
    <div v-else>🥤, 🍺 &amp; 🍷, 🍸</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      age: "",
      inputField: "dummyjjj",
      product: {
        name: "Socks",
        inStock: true,
        onSale: false,
      },
    };
  },
};
</script>
