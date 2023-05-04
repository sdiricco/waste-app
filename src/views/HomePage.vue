/* eslint-disable */

<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">

        <ion-tab-button tab="overview" href="/home/overview">
          <ion-icon :icon="calendarOutline" />
          <ion-label>Esposizione</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="categories" href="/home/categories">
          <ion-icon :icon="layersOutline" />
          <ion-label>Categorie</ion-label>
        </ion-tab-button>
          
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script lang="ts" setup>
/* Ionic components */
import { 
  IonTabBar,
  IonTabButton,
  IonTabs,
  IonLabel,
  IonIcon,
  IonPage,
  IonRouterOutlet 
} from '@ionic/vue';
import { 
  layersOutline,
  calendarOutline
} from 'ionicons/icons';

</script>
