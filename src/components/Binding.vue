<template>
  <h1>Binding</h1>
  <div>
    My favorite YouTubeChannel is
    <a :href="youTubeChannel">{{ youTubeChannel }}</a>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      youTubeChannel:
        "https://www.youtube.com/channel/UCsBjURrPoezykLs9EqgamOA",
    };
  },
};
</script>
