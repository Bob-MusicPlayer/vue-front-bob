<template>
    <div>
      <button :class="{circle: circle}">
        <font-awesome-icon fixed-width :size="size" :style="{color: color}" :icon="icon" />
      </button>
    </div>
</template>

<script>
    export default {
        name: "IconButton",
        props: {
            icon: String,
            circle: Boolean,
            size: {
                type: String,
                default: "lg"
            },
            color: {
                type: String,
                default: "#fff"
            }
        }
    }
</script>

<style scoped>
  button {
    background-color: transparent;
    color: white;
    border: none;
    padding: 10px;
    width: 40px;
    height: 40px;
  }

  button:focus {
    outline: none;
  }

  button:hover:not(.circle)>svg {
    color: #8fb3cb;
  }

  button.circle {
    border: 1px solid #787878;
    border-radius: 50%;
  }

  button.circle:hover {
    border-color: #8fb3cb;
    box-shadow: 0 2px 10px 0 #092d47;
  }
</style>
