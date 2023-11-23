<script setup lang="ts">
const imgUrl =
  "https://images.unsplash.com/photo-1438761681033-6461ffad8d80?q=80&w=2670&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D";
const alt = "profile";
const tooltip = "UserName";
</script>

<template>
  <div>
    <v-tooltip location="bottom">
      <template v-slot:activator="{ props }">
        <v-avatar v-bind="props" style="cursor: pointer">
          <v-img
            class="bg-white"
            width="300"
            :aspect-ratio="1"
            :src="imgUrl"
            cover
          ></v-img>
        </v-avatar>
      </template>
      <span>{{ tooltip }}</span>
    </v-tooltip>
  </div>
</template>

<style></style>
