/* eslint-disable */

<template>
  <ion-page>
    <ion-content :fullscreen="true">
      <ion-card>
        <ion-card-header>
          <ion-card-title>{{ title }}</ion-card-title>
          <ion-card-subtitle>{{ subtitle }}</ion-card-subtitle>
        </ion-card-header>

        <ion-card-content>
          <ion-list>
            <ion-item v-for="(item, index) in items" :key="index">
              <ion-avatar slot="start">
                <img :src="item.avatar" />
              </ion-avatar>
              <ion-label>{{ item.name }}</ion-label>
            </ion-item>
          </ion-list>
          <ion-range></ion-range>
        </ion-card-content>
      </ion-card>
    </ion-content>
  </ion-page>
</template>

<script lang="ts" setup>
import { IonCard, IonRange, IonCardHeader, IonCardTitle, IonCardSubtitle, IonCardContent, IonContent, IonHeader, IonPage, IonList, IonItem, IonAvatar, IonLabel } from "@ionic/vue";
import SearchToolbar from "@/components/SearchToolbar.vue";
import { ref } from "vue";

const title = ref("Title");
const subtitle = ref("Subtitle");

const items = ref([
  {
    name: 'Utente 1',
    avatar: 'https://via.placeholder.com/64', // Immagine presa da internet (immagine generica)
  },
  {
    name: 'Utente 2',
    avatar: 'https://via.placeholder.com/64',
  },
  {
    name: 'Utente 3',
    avatar: 'https://via.placeholder.com/64',
  },
]);
</script>

<style scoped>
ion-range {
  --bar-background: #a2d2ff;
  --bar-background-active: #bde0fe;
  --bar-height: 8px;
  --bar-border-radius: 8px;
  --knob-background: #ffc8dd;
  --knob-size: 40px;
  --pin-background: #ffafcc;
  --pin-color: #fff;
}
</style>
