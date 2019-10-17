<template>
  <div class="grid-container">
    <div class="sidebar">
      <Sidebar />
    </div>
    <div class="main">
      <nuxt />
    </div>
    <div class="player_track">
      <PlayerTrack />
    </div>
    <div class="player_controls">
      <PlayerControls />
    </div>
  </div>
</template>

<style>
html, body {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
  height: 100%;
  width: 100%;
  margin: 0;
  background-color: #1a1927;
  color: white;
}

#__layout {
  height: 100%;
}

#__nuxt {
  height: 100%;
}

.grid-container {
  height: 100%;
  display: grid;
  grid-template-columns: auto 1fr;
  grid-template-rows: 1fr auto;
  grid-template-areas: "sidebar main" "player_track player_controls";
}

.sidebar { grid-area: sidebar; }

.main { grid-area: main; }

.player_track { grid-area: player_track; }

.player_controls { grid-area: player_controls; }
</style>
<script>
    import Sidebar from "../components/Sidebar";
    import PlayerTrack from "../components/PlayerTrack";
    import PlayerControls from "../components/PlayerControls";
    export default {
        components: {PlayerControls, PlayerTrack, Sidebar}
    }
</script>
