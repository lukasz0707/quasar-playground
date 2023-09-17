<script setup>
import { reactive } from "vue";
import TodoCreateButton from "components/TodoCreateButton.vue";

const state = reactive({
  search: "",
  checkbox: true,
});
</script>

<template>
  <q-page class="row">
    <!-- <div class="bg-blue col-3" style="height: 22px" />
    <div class="bg-purple col-3" style="height: 22px" />
    <div class="bg-green col-6" style="height: 22px" /> -->
    <q-card class="col-xs-9">
      <q-toolbar>
        <q-input
          dense
          placeholder="Search"
          borderless
          class="full-width"
          v-model="state.search"
        >
          <template #append> <q-icon name="mdi-magnify" /> </template>
        </q-input>
      </q-toolbar>
      <q-list bordered>
        <q-item>
          <q-item-section side>
            <q-checkbox v-model="state.checkbox"></q-checkbox>
          </q-item-section>
          <q-item-section> Go Shopping </q-item-section>
          <q-item-section side>
            <q-btn icon="mdi-delete" flat round size="md" />
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
    <div class="col-xs-3">
      <q-toolbar class="bg-primary">
        <TodoCreateButton />
      </q-toolbar>
    </div>
  </q-page>
</template>

<style scoped lang="scss"></style>
