<template>
  <div class="rec-border" :style="cssVars"></div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'RectanguloRedondo',
  props: {
    width: {
      type: Number,
      default: 100,
    },
    color: {
      type: String,
      default: 'red',
    },
    rotate: {
      type: Number,
      default: 0,
    },
    top: {
      type: Number,
      default: 0,
    },
    right: {
      type: Number,
      default: 0,
    },
  },
  setup() {
    return {};
  },
  computed: {
    cssVars() {
      return {
        width: `${this.$props.width}px`,
        'background-color': this.color,
        rotate: `${this.$props.rotate}deg`,
        top: `${this.top}%`,
        right: `${this.right}%`,
      };
    },
  },
});
</script>

<style lang="scss">
.rec-border {
  // width: 500px;
  height: 70px;
  border-top-left-radius: 100px;
  border-bottom-left-radius: 100px;
  border-top-right-radius: 100px;
  border-bottom-right-radius: 100px;
  position: fixed;

  // background-color: red;
}
</style>
