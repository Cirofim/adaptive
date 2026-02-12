<script setup>
import logo from "@/components/Logo.vue";
import navigation from "@/components/navigation.vue";
import photoo from "./components/Photoo.vue";
import Info from "./components/Info.vue"
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
