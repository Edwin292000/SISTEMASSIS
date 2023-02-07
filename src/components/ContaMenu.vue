<template>
  <q-expansion-item
    expand-separator
    icon="perm_identity"
    label="Contabilidad"
    caption="John Doe"
  >
    <q-expansion-item
      :header-inset-level="1"
      expand-separator
      icon="perm_identity"
      label="CxP"
      caption=""
    >
      <q-list bordered>
        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon color="primary" name="bluetooth" />
          </q-item-section>
          <q-item-section>Icon as avatar</q-item-section>
        </q-item>
      </q-list>
    </q-expansion-item>
    <q-expansion-item
      :header-inset-level="1"
      expand-separator
      icon="perm_identity"
      label="CxC"
      caption=""
    >
      <q-list bordered>
        <q-item clickable v-ripple>
          <q-item-section avatar>
            <q-icon color="primary" name="bluetooth" />
          </q-item-section>
          <q-item-section>Icon as avatar</q-item-section>
        </q-item>
      </q-list>
    </q-expansion-item>
  </q-expansion-item>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
export default defineComponent({
  name: 'ContaMenu',
  setup() {
    return {};
  },
});
</script>
