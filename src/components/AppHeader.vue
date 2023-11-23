<script setup lang="ts">
import AvatarImg from '@/components/atoms/AvatarImg.vue'
import { customLightTheme, APP_CONST } from '@/commons'
</script>

<template>
  <v-app-bar :color="customLightTheme.colors?.primary">
    <template v-slot:prepend>
      <v-app-bar-nav-icon />
    </template>

    <v-app-bar-title>{{ APP_CONST.title }}</v-app-bar-title>

    <v-spacer />

    <v-btn icon>
      <AvatarImg />
    </v-btn>

  </v-app-bar>
</template>

<style></style>
