<script setup>
import logo from "@/components/Logo.vue";
import navigation from "@/components/navigation.vue";
import photoo from "./components/Photoo.vue";
</script>

<template>
  <header>
    <logo />
    <navigation />
  </header>

  <main>
    <photoo />
  </main>
</template>

<style lang="scss" module>
header {
  width: 64rem;
  margin: 0 auto;
}
</style>
