<template>
  <ion-app>
    <ion-page >
      <ion-router-outlet />
    </ion-page>
  </ion-app>
</template>

<script lang="ts" setup>
import { IonApp, IonRouterOutlet, IonPage, IonMenu } from "@ionic/vue";
import  SiderBar from './components/SideBar.vue'
import { onMounted } from "vue";
import { useStore } from "@/store/main";


const store = useStore();
onMounted(async () => {
  await store.loadApp();
  store.$subscribe(async (_mutations, state) => {
    await store.savePreferences(state.preferences);
  });
});
</script>

<style>
@import './main.css'
</style>
