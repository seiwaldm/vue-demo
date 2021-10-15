<template>
  <h1>List Rendering</h1>
  <p>Eine Liste mit empfehlenswerten YouTube-Channels:</p>
  <ul>
    <li v-for="link in linkList" v-bind:key="link.name">
      <a v-bind:href="link.link">{{ link.name }}</a>
    </li>
  </ul>
</template>

<script>
export default {
  data: function() {
    return {
      linkList: [
        {
          name: "Firebase.io Channel",
          link: "https://www.youtube.com/channel/UCsBjURrPoezykLs9EqgamOA",
        },
        {
          name: "Traversy Media Channel",
          link: "https://www.youtube.com/user/TechGuyWeb/",
        },
      ],
    };
  },
};
</script>
