<template>
    <div class="wrapper">
      <div class="wrapper_pn pn_left">
        <span class="header">PREVIOUS</span>
        <span>Podobny</span>
      </div>
      <div class="actions">
        <IconButton icon="random" color="#787a89" />
        <IconButton icon="step-backward" color="#787a89" />
        <IconButton icon="play" circle color="#b5b8c9" />
        <IconButton icon="step-forward" color="#787a89" />
        <IconButton icon="sync-alt" color="#787a89" />
      </div>
      <div class="wrapper_pn pn_right">
        <span class="header">NEXT</span>
        <span>More than you know</span>
      </div>
    </div>
</template>

<script>
    import IconButton from "./IconButton";
    export default {
        name: "PlayerControls",
        components: {IconButton}
    }
</script>

<style scoped>
  .wrapper {
    background-color: #23232f;
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-between;
  }

  .wrapper_pn {
    display: flex;
    flex-direction: column;
  }

  .pn_left {
    padding-left: 30px;
    padding-top: 20px;
  }

  .pn_right {
    padding-right: 30px;
    padding-top: 20px;
    text-align: right;
  }

  .wrapper_pn > .header {
    color: #787878;
    font-size: .8rem;
  }

  .actions {
    display: flex;
  }
</style>
