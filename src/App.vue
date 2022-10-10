<template>
  <q-layout view="lHh Lpr lFf">
    <SideBar />
    <RightSideBar />
    <q-page-container>
      <router-view></router-view>
    </q-page-container>
  </q-layout>
</template>

<script setup>
/* eslint-disable */
import { ref } from "vue";
import RightSideBar from "./components/RightSideBar.vue";
import SideBar from "./components/SideBar.vue";
const leftDrawerOpen = ref(false);
</script>
