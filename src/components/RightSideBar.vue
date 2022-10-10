<template>
  <q-drawer
    show-if-above
    v-model="rightDrawerOpen"
    side="right"
    bordered
    :width="240"
  >
    <q-toolbar class="q-mt-lg">
      <q-icon name="far fa-question-circle" class="q-mr-sm"></q-icon>
      <q-icon name="far fa-caret-square-right"></q-icon>
      <q-space></q-space>
      <q-icon name="fab fa-mixcloud" class="q-mr-sm"></q-icon>
      <div class="text-overline">Online</div>
    </q-toolbar>

    <div class="flex flex-center column">
      <q-item class="q-mx-sm">
        <q-item-section avatar>
          <q-avatar>
            <img src="https://github.com/BrunoYottabyte.png" />
          </q-avatar>
        </q-item-section>

        <q-item-section class="none">
          <div>
            <strong>Bruno Siqueira</strong>
            <q-badge color="green" rounded class="q-mx-sm"></q-badge>
            <q-icon name="fas fa-chevron-down"></q-icon>
          </div>
          <q-item-label caption>Bruno762</q-item-label>
        </q-item-section>
      </q-item>
      <div class="text-h6">
        <strong>150.080.01</strong>
        <q-icon
          name="fas fa-plus-circle"
          color="green"
          class="q-ml-md"
        ></q-icon>
      </div>
    </div>
    <q-toolbar>
      <q-icon name="fas fa-info-circle" class="q-mr-sm"></q-icon>
      <div class="text-overline">Zap Coins</div>
    </q-toolbar>

    <div class="flex flex-center column q-pa-md">
      <q-linear-progress rounded size="20px" value="0.69" color="warning" />
      <q-toolbar class="top">
        <div class="text-overline">Storage</div>
        <q-space></q-space>
        <div class="text-overline">69%</div>
      </q-toolbar>
    </div>
    <q-toolbar class="top">
      <q-icon name="far fa-hdd" class="q-mr-sm" />
      <div class="text-overline">Partner Menu</div>
    </q-toolbar>
    <q-separator />
    <q-toolbar>
      <q-icon name="fas fa-columns" class="q-mr-sm"> </q-icon>
      <div class="text-overline">Web interface</div>
    </q-toolbar>

    <q-toolbar class="top">
      <q-icon name="fas fa-sitemap" class="q-mr-sm"> </q-icon>
      <div class="text-overline">Website</div>
    </q-toolbar>

    <q-toolbar class="top">
      <q-icon name="fas fa-check-square" class="q-mr-sm"> </q-icon>
      <div class="text-overline">Ticket support</div>
    </q-toolbar>

    <q-toolbar class="top">
      <q-icon name="fab fa-figma" class="q-mr-sm"> </q-icon>
      <div class="text-overline">Interruptions</div>
    </q-toolbar>

    <q-toolbar class="top">
      <q-icon name="fab fa-chrome" class="q-mr-sm"> </q-icon>
      <div class="text-overline">Donation settings</div>
    </q-toolbar>

    <q-toolbar class="top">
      <q-icon name="far fa-star" class="q-mr-sm"> </q-icon>
      <div class="text-overline">Wish list</div>
    </q-toolbar>

    <div
      style="
        position: absolute;
        bottom: 20px;
        margin-left: auto;
        margin-right: auto;
        left: 0;
        right: 0;
        text-align: center;
      "
    >
      <div class="flex flex-center row">
        <div class="text-overline">Quick news</div>
        <q-icon name="fab fa-facebook-f" class="q-mx-md"></q-icon>
        <q-icon name="fab fa-twitter"></q-icon>
      </div>
    </div>
  </q-drawer>
</template>

<script setup>
/*eslint-disable*/
import { ref } from "vue";
const rightDrawerOpen = ref(false);
</script>

<style>
.q-item__section--main.none {
  flex: none !important;
}

.top {
  margin-top: -10px;
}
</style>
