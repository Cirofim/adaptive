<script setup>
import logo from "@/components/logo.vue";
import navigation from "@/components/navigation.vue";
import photoo from "./components/photoo.vue"
</script>

<template>
  <header>
    <logo />
    <navigation />
  </header>

  <main>
    <photoo/>


  </main>

</template>

<style lang="scss">
@import url(./assets/global/style.scss);
</style>
