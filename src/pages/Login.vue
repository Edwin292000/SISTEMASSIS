<template>
  <div class="fullscreen bg-blue">
    <BackgroundLogin></BackgroundLogin>
    <q-card
      class="fixed-center shadow-10 bg-grey-9 card-login q-pa-sm"
      style="width: 30%"
    >
      <div class="bg-red full-width">
        <Transition
          appear
          enter-active-class="animated bounceIn"
          :duration="3000"
        >
          <q-avatar
            size="70px"
            font-size="50px"
            color="dark"
            text-color="white"
            icon="person"
            class="absolute"
            style="right: 40%; top: -30px"
          />
        </Transition>
      </div>
      <q-card-section>
        <br />
        <div class="text-h6 text-center q-pb-none">Login</div>
        <q-separator dark />
      </q-card-section>
      <q-tabs v-model="tab">
        <q-tab name="ventas" icon="point_of_sale" label="Ventas" />
        <q-tab name="admin" icon="manage_accounts" label="Admin" />
      </q-tabs>
      <!-- <q-card-section class="q-pa-none">
        <br /><br />
        <div class="text-h6 text-center q-pb-none">Login</div>
        <q-separator spaced dark />
      </q-card-section> -->
      <q-tab-panels v-model="tab" animated>
        <q-tab-panel name="ventas">
          <q-card-section>
            <q-input
              v-model="text"
              type="text"
              label="Vendedor"
              standout
              dense
              rounded
            />
            <br />
            <q-input
              v-model="text"
              type="text"
              label="Contraseña"
              standout
              dense
              rounded
            />
            <br />
            <div class="row justify-center">
              <q-btn
                color="primary"
                label="Ingresar"
                @click="onClick"
                rounded
              />
            </div>
          </q-card-section>
        </q-tab-panel>
        <q-tab-panel name="admin">
          <q-card-section>
            <q-input
              v-model="text"
              type="text"
              label="Usuario"
              standout
              dense
              rounded
            />
            <br />
            <q-input
              v-model="text"
              type="text"
              label="Contraseña"
              standout
              dense
              rounded
            />
            <br />
            <div class="row justify-center">
              <q-btn
                color="primary"
                label="Ingresar admin"
                @click="onClick"
                rounded
              />
            </div>
          </q-card-section>
        </q-tab-panel>
      </q-tab-panels>
    </q-card>
  </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
import BackgroundLogin from 'components/BackgroundLogin.vue';
export default defineComponent({
  name: 'loginPage',
  components: {
    BackgroundLogin,
  },
  setup() {
    return {
      tab: ref('ventas'),
    };
  },
});
</script>

<style lang="scss">
.card-login {
  border-radius: 25px;
}
</style>
