<template>
  <q-expansion-item expand-separator icon="perm_identity" label="Inventario">
    <q-list bordered>
      <q-item clickable v-ripple>
        <q-item-section>
          <q-item-label>Productos</q-item-label>
          <!-- <q-item-label caption lines="2">Secondary line text.</q-item-label> -->
        </q-item-section>
      </q-item>
      <q-separator />
      <q-item clickable v-ripple>
        <q-item-section>
          <q-item-label>Lotes</q-item-label>
          <!-- <q-item-label caption lines="2">Secondary line text.</q-item-label> -->
        </q-item-section>
      </q-item>
    </q-list>
  </q-expansion-item>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'InventarioMenu',
});
</script>
