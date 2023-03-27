<template>
  <ion-app>
    <ion-page >
      <ion-router-outlet />
    </ion-page>
  </ion-app>
</template>

<script lang="ts" setup>
import { IonApp, IonRouterOutlet, IonPage } from "@ionic/vue";
</script>

<style>
@import './main.css'
</style>
