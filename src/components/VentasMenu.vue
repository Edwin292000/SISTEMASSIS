<template>
  <q-expansion-item
    expand-separator
    icon="perm_identity"
    label="Ventas"
    caption=""
  >
    <q-list bordered>
      <q-item clickable v-ripple>
        <q-item-section>
          <q-item-label>Series</q-item-label>
        </q-item-section>
      </q-item>
      <q-separator />
      <q-item>
        <q-item-section>
          <q-item-label>Vendedores</q-item-label>
        </q-item-section>
      </q-item>
    </q-list>
  </q-expansion-item>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'VentasMenu',
  setup() {
    return {};
  },
});
</script>
