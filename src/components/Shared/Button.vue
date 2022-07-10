<template>
  <button type='button' class='button' :style='cssVars' @click='$router.push(`/${route}`)'>{{text}}</button>
</template>

<script>
export default {
  props: {
    text: String,
    color: String,
    hover: String,
    active: String,
    route: String
  },
  computed: {
    cssVars() {
      return {
        '--bg-color': this.color,
        '--bg-color-hover': this.hover,
        '--bg-color-active': this.active,
      }
    }
  }
}
</script>

<style scoped>
.button {
  align-items: center;
  background-clip: padding-box;
  /* background-color: #fa6400; */
  background-color: var(--bg-color);
  border: 1px solid transparent;
  border-radius: .25rem;
  box-shadow: rgba(0, 0, 0, 0.02) 0 1px 3px 0;
  box-sizing: border-box;
  color: #fff;
  cursor: pointer;
  display: inline-flex;
  font-family: system-ui,-apple-system,system-ui,"Helvetica Neue",Helvetica,Arial,sans-serif;
  font-size: 16px;
  font-weight: 600;
  justify-content: center;
  line-height: 1.25;
  margin: 0;
  min-height: 3rem;
  padding: calc(.875rem - 1px) calc(1.5rem - 1px);
  position: relative;
  text-decoration: none;
  transition: all 250ms;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  vertical-align: baseline;
  width: auto;
}
.button:hover,
.button:focus {
  /* background-color: #fb8332; */
  background-color: var(--bg-color-hover);
  box-shadow: rgba(0, 0, 0, 0.1) 0 4px 12px;
}
.button:hover {
  transform: translateY(-1px);
}
.button:active {
  /* background-color: #c85000; */
  background-color: var(--bg-color-active);
  box-shadow: rgba(0, 0, 0, .06) 0 2px 4px;
  transform: translateY(0);
}
</style>