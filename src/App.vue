<script setup>
import { RouterView } from 'vue-router'
import Navigation from "@/components/Navigation.vue";
import SeoTeleport from "@/components/SeoTeleport.vue";
</script>

<template>
  <seo-teleport />
  <navigation />
  <RouterView />
</template>
