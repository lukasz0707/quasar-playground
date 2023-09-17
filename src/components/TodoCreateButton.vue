<script setup>
//import {} from 'vue'

function doSomething() {
  alert("did something!");
}
</script>

<template>
  <q-btn
    @click="doSomething"
    fab
    color="secondary"
    style="margin-bottom: -42px"
    icon="mdi-plus"
    class="q-ml-lg"
  ></q-btn>
</template>

<style scoped lang="scss"></style>
