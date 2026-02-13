<script setup>
import logo from "@/components/Top_logo.vue";
import navigation from "@/components/Low_logo.vue";
import photoo from "./components/Block_with_photos.vue";
import Info from "./components/Descrption_about_room.vue"
</script>

<template>
  <header>
    <logo />
    <navigation />
  </header>

  <main>
    <photoo />
    <Info/>
    
  </main>
</template>

<style lang="scss" module></style>
