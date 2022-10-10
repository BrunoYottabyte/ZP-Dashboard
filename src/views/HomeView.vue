<template>
  <div class="q-pa-md">
    <div class="row q-col-gutter-md">
      <div class="col-4">
        <AccountDash />
      </div>
      <div class="col-8">
        <div class="row q-col-gutter-md">
          <div class="col-10">
            <q-card class="my-card q-px-sm" flat bordered>
              <q-toolbar>
                <q-icon name="fas fa-archive" class="q-mr-sm"></q-icon>
                <div class="text-overline q-mr-sm">Voucher</div>
                <q-badge
                  label="8"
                  rounded
                  color="green"
                  class="q-mr-sm"
                ></q-badge>

                <q-icon name="fas fa-user" class="q-mr-sm"></q-icon>
                <div class="text-overline q-mr-sm">Partner</div>
                <q-badge label="6" rounded color="green"></q-badge>

                <q-icon name="fas fa-shield-alt" class="q-mx-sm"></q-icon>
                <div class="text-overline q-mr-sm">Support</div>
                <q-space></q-space>
                <q-btn
                  color="green"
                  icon="fab fa-mixcloud"
                  label="On Left"
                ></q-btn>
              </q-toolbar>
            </q-card>
          </div>

          <div class="col-2">
            <q-card class="my-card q-px-sm" flat bordered>
              <q-toolbar class="flex flex-center column">
                <q-icon name="fas fa-ellipsis-h" class="q-mx-sm"></q-icon>
              </q-toolbar>
            </q-card>
          </div>
        </div>
        <h6 class="text-weight-bolder q-ml-lg topTitle">Dashboard</h6>
        <q-toolbar class="topToolbar">
          <div class="text-overline q-mr-sm">My Gameservers</div>
          <q-badge label="28" rounded color="grey" class="q-mr-sm"></q-badge>
          <div class="text-overline q-mx-sm">My VPS</div>
          <q-badge label="10" rounded color="grey"></q-badge>
          <div class="text-overline q-mx-sm">My Rootservers</div>
          <q-badge label="29" rounded color="grey"></q-badge>
          <div class="text-overline q-mx-sm">My Domains</div>
          <q-badge label="5" rounded color="grey"></q-badge>
          <q-space></q-space>

          <q-icon name="fas fa-ellipsis-h" class="q-mx-sm"></q-icon>
        </q-toolbar>

        <div class="row q-col-gutter-md">
          <div class="col-4">
            <q-card class="my-card q-px-sm q-py-lg secCard card1">
              <q-toolbar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar1.jpg" />
                </q-avatar>
                <q-space></q-space>
                <q-badge label="Online" rounded color="green"></q-badge>
              </q-toolbar>

              <div class="text-overline text-weight-bolder q-ml-md">
                Fivem Dev #256019
              </div>
              <div class="text-overline q-ml-md">185.223.28.170.2000</div>
              <q-toolbar>
                <div class="text-overline text-weight-bolder q-ml-sm">
                  21.11.2022
                </div>
                <q-space></q-space>
                <q-btn
                  color="grey"
                  round
                  flat
                  dense
                  :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
                  @click="expanded = !expanded"
                ></q-btn>
              </q-toolbar>
              <q-separator></q-separator>
              <q-slide-transition>
                <div v-show="expanded">
                  <q-card-section class="flex flex-center row">
                    <q-icon name="far fa-lightbulb" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-laptop" class="q-mr-md"></q-icon>
                    <q-icon name="far fa-credit-card" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-box" class="q-mr-md"></q-icon>
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-4">
            <q-card class="my-card q-px-sm q-py-lg secCard card2">
              <q-toolbar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar2.jpg" />
                </q-avatar>
                <q-space></q-space>
                <q-badge label="Online" rounded color="green"></q-badge>
              </q-toolbar>

              <div class="text-overline text-weight-bolder q-ml-md">
                Fivem Dev #256019
              </div>
              <div class="text-overline q-ml-md">185.223.28.170.2000</div>
              <q-toolbar>
                <div class="text-overline text-weight-bolder q-ml-sm">
                  21.11.2022
                </div>
                <q-space></q-space>
                <q-btn
                  color="grey"
                  round
                  flat
                  dense
                  :icon="
                    expanded2 ? 'keyboard_arrow_up' : 'keyboard_arrow_down'
                  "
                  @click="expanded2 = !expanded2"
                ></q-btn>
              </q-toolbar>
              <q-separator></q-separator>
              <q-slide-transition>
                <div v-show="expanded2">
                  <q-card-section class="flex flex-center row">
                    <q-icon name="far fa-lightbulb" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-laptop" class="q-mr-md"></q-icon>
                    <q-icon name="far fa-credit-card" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-box" class="q-mr-md"></q-icon>
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-4">
            <q-card class="my-card q-px-sm q-py-lg secCard card3">
              <q-toolbar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar3.jpg" />
                </q-avatar>
                <q-space></q-space>
                <q-badge label="Online" rounded color="green"></q-badge>
              </q-toolbar>

              <div class="text-overline text-weight-bolder q-ml-md">
                Fivem Dev #256019
              </div>
              <div class="text-overline q-ml-md">185.223.28.170.2000</div>
              <q-toolbar>
                <div class="text-overline text-weight-bolder q-ml-sm">
                  21.11.2022
                </div>
                <q-space></q-space>
                <q-btn
                  color="grey"
                  round
                  flat
                  dense
                  :icon="
                    expanded3 ? 'keyboard_arrow_up' : 'keyboard_arrow_down'
                  "
                  @click="expanded3 = !expanded3"
                ></q-btn>
              </q-toolbar>
              <q-separator></q-separator>
              <q-slide-transition>
                <div v-show="expanded3">
                  <q-card-section class="flex flex-center row">
                    <q-icon name="far fa-lightbulb" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-laptop" class="q-mr-md"></q-icon>
                    <q-icon name="far fa-credit-card" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-box" class="q-mr-md"></q-icon>
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-4">
            <q-card class="my-card q-px-sm q-py-lg secCard card4">
              <q-toolbar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar4.jpg" />
                </q-avatar>
                <q-space></q-space>
                <q-badge label="Online" rounded color="green"></q-badge>
              </q-toolbar>

              <div class="text-overline text-weight-bolder q-ml-md">
                Fivem Dev #256019
              </div>
              <div class="text-overline q-ml-md">185.223.28.170.2000</div>
              <q-toolbar>
                <div class="text-overline text-weight-bolder q-ml-sm">
                  21.11.2022
                </div>
                <q-space></q-space>
                <q-btn
                  color="grey"
                  round
                  flat
                  dense
                  :icon="
                    expanded4 ? 'keyboard_arrow_up' : 'keyboard_arrow_down'
                  "
                  @click="expanded4 = !expanded4"
                ></q-btn>
              </q-toolbar>
              <q-separator></q-separator>
              <q-slide-transition>
                <div v-show="expanded4">
                  <q-card-section class="flex flex-center row">
                    <q-icon name="far fa-lightbulb" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-laptop" class="q-mr-md"></q-icon>
                    <q-icon name="far fa-credit-card" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-box" class="q-mr-md"></q-icon>
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-4">
            <q-card class="my-card q-px-sm q-py-lg secCard card5">
              <q-toolbar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar5.jpg" />
                </q-avatar>
                <q-space></q-space>
                <q-badge label="Online" rounded color="green"></q-badge>
              </q-toolbar>

              <div class="text-overline text-weight-bolder q-ml-md">
                Fivem Dev #256019
              </div>
              <div class="text-overline q-ml-md">185.223.28.170.2000</div>
              <q-toolbar>
                <div class="text-overline text-weight-bolder q-ml-sm">
                  21.11.2022
                </div>
                <q-space></q-space>
                <q-btn
                  color="grey"
                  round
                  flat
                  dense
                  :icon="
                    expanded5 ? 'keyboard_arrow_up' : 'keyboard_arrow_down'
                  "
                  @click="expanded5 = !expanded5"
                ></q-btn>
              </q-toolbar>
              <q-separator></q-separator>
              <q-slide-transition>
                <div v-show="expanded5">
                  <q-card-section class="flex flex-center row">
                    <q-icon name="far fa-lightbulb" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-laptop" class="q-mr-md"></q-icon>
                    <q-icon name="far fa-credit-card" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-box" class="q-mr-md"></q-icon>
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
          <div class="col-4">
            <q-card class="my-card q-px-sm q-py-lg secCard card6">
              <q-toolbar>
                <q-avatar>
                  <img src="https://cdn.quasar.dev/img/avatar6.jpg" />
                </q-avatar>
                <q-space></q-space>
                <q-badge label="Online" rounded color="green"></q-badge>
              </q-toolbar>

              <div class="text-overline text-weight-bolder q-ml-md">
                Fivem Dev #256019
              </div>
              <div class="text-overline q-ml-md">185.223.28.170.2000</div>
              <q-toolbar>
                <div class="text-overline text-weight-bolder q-ml-sm">
                  21.11.2022
                </div>
                <q-space></q-space>
                <q-btn
                  color="grey"
                  round
                  flat
                  dense
                  :icon="
                    expanded6 ? 'keyboard_arrow_up' : 'keyboard_arrow_down'
                  "
                  @click="expanded6 = !expanded6"
                ></q-btn>
              </q-toolbar>
              <q-separator></q-separator>
              <q-slide-transition>
                <div v-show="expanded6">
                  <q-card-section class="flex flex-center row">
                    <q-icon name="far fa-lightbulb" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-laptop" class="q-mr-md"></q-icon>
                    <q-icon name="far fa-credit-card" class="q-mr-md"></q-icon>
                    <q-icon name="fas fa-box" class="q-mr-md"></q-icon>
                  </q-card-section>
                </div>
              </q-slide-transition>
            </q-card>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
/* eslint-disable */
import { ref } from "vue";
import AccountDash from "@/components/AccountDash.vue";
const expanded = ref(false);
const expanded6 = ref(false);
const expanded2 = ref(false);
const expanded3 = ref(false);
const expanded4 = ref(false);
const expanded5 = ref(false);
</script>

<style scoped>
.topTitle {
  margin-top: 10px;
}

.topToolbar {
  margin-top: -40px;
}

.secCard {
  border-radius: 20px;
}

.card1 {
  background: #edfef0;
}

.card2 {
  background: #fef8ea;
}

.card3 {
  background: #f6f8f7;
}

.card4 {
  background: #81ecec;
}

.card5 {
  background: #fab1a0;
}

.card6 {
  background: #ffeaa7;
}
</style>
