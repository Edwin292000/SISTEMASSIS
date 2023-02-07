<template>
  <div class="fit">
    <br />
    <RectanguloRedondo :width="1000" :rotate="150" :top="-10" :right="-39" />
    <RectanguloRedondo :width="1000" :rotate="150" :top="-10" :right="-39" />
    <RectanguloRedondo :width="1000" :rotate="150" :top="-10" :right="-25" />
    <RectanguloRedondo :width="1000" :rotate="150" :top="-10" :right="-53" />
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import RectanguloRedondo from 'components/RectanguloRedondo.vue';
export default defineComponent({
  name: 'BackgroundLogin',
  components: {
    RectanguloRedondo,
  },
});
</script>
