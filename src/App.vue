<template>
  <navBar />
  <router-view />
  <img src="@/assets/images/sidefixe.png" class="sidefixe" />
</template>

<script setup>
import navBar from "@/components/navBar.vue";
</script>


<style lang="scss" >
#app {
  overflow-x: hidden;
}
</style>