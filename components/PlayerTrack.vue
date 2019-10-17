<template>
  <div class="wrapper">
    <div class="track_img"></div>
    <div class="track_info">
      <span>Walking the wire</span>
      <span class="track_author">Imagine Dragons</span>
    </div>
  </div>
</template>

<script>
    export default {
        name: "PlayerTrack"
    }
</script>

<style scoped>
  .wrapper {
    background-color: #272634;
    padding: 15px 30px;
    display: flex;
    align-items: center;
  }

  .track_img {
    background-image: url("https://upload.wikimedia.org/wikipedia/en/e/e9/Imagine_Dragons_Walking_the_Wire.jpg");
    background-size: cover;
    border-radius: 10%;
    height: 52px;
    width: 52px;
  }

  .track_info {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-left: 10px;
  }

  .track_author {
    color: #787878;
    font-size: .8rem;
  }
</style>
