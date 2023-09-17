<script setup>
import { ref } from "vue";

const checked = ref(false);
const email = ref("");
const password = ref("");
</script>

<template>
  <q-page class="flex flex-center" padding>
    <div class="full-width" style="max-width: 300px">
      <h5 class="q-my-md text-center">Login</h5>
      <q-card>
        <q-card-section>
          <q-form>
            <q-input
              v-model="email"
              label="email"
              placeholder="email@example.com"
              filled
              class="q-mb-md"
            ></q-input>
            <q-input
              v-model="password"
              label="password"
              type="password"
              class="q-mb-xs"
              filled
            ></q-input>
            <q-checkbox label="remember me" v-model="checked"></q-checkbox>
            <q-btn
              label="login"
              class="full-width q-mt-md"
              color="primary"
            ></q-btn>
          </q-form>
        </q-card-section>
      </q-card>
    </div>
  </q-page>
</template>

<style scoped lang="scss"></style>
