/* eslint-disable */

<template>
  <ion-page class="ion-padding">
    <ion-accordion-group expand="inset">
      <ion-accordion value="first">
        <ion-item slot="header" color="light">
          <ion-text>
            <h3>Martedì 24/05</h3>
          </ion-text>
        </ion-item>
        <div class="ion-padding" slot="content">
          <ion-text color="medium">
            <p>Martedì 24 maggio 2023</p>
          </ion-text>
          <ion-text>
            <p>Oggi ricordati di esporre fuori il Secco e la Plastica</p>
          </ion-text>
          <div class="waste-container">
            <div class="waste">
              <div class="icon"></div>
              <div class="label">Secco</div>
            </div>
            <div class="waste">
              <div class="icon"></div>
              <div class="label">Plastica</div>
            </div>
          </div>
          <div class="footer">
            <ion-icon :icon="timeOutline" size="large"></ion-icon>
            <ion-text class="pl-8"> Orario di presa in carico stimato per le 06:30 </ion-text>
          </div>
        </div>
      </ion-accordion>
      <ion-accordion value="second">
        <ion-item slot="header" color="light">
          <ion-text>
            <h3>Mercoledì 25/05</h3>
          </ion-text>
        </ion-item>
        <div class="ion-padding" slot="content">
          <ion-text color="medium">
            <p>Mercoledì 25 maggio 2023</p>
          </ion-text>
          <ion-text>
            <p>Oggi ricordati di esporre fuori l'indifferenziata</p>
          </ion-text>
          <div class="waste-container">
            <div class="waste">
              <div class="icon"></div>
              <div class="label">Indifferenziata</div>
            </div>
          </div>
          <div class="footer">
            <ion-icon :icon="timeOutline" size="large"></ion-icon>
            <ion-text class="pl-8"> Orario di presa in carico stimato per le 06:30 </ion-text>
          </div>
        </div>
      </ion-accordion>
      <ion-accordion value="third">
        <ion-item slot="header" color="light">
          <ion-text>
            <h3>Giovedì 26/05</h3>
          </ion-text>
        </ion-item>
        <div class="ion-padding" slot="content">
          <ion-text color="medium">
            <p>Giovedì 26 maggio 2023</p>
          </ion-text>
          <ion-text>
            <p>Oggi ricordati di esporre fuori il Vetro</p>
          </ion-text>
          <div class="waste-container">
            <div class="waste">
              <div class="icon"></div>
              <div class="label">Vetro</div>
            </div>
          </div>
          <div class="footer">
            <ion-icon :icon="timeOutline" size="large"></ion-icon>
            <ion-text class="pl-8"> Orario di presa in carico stimato per le 06:30 </ion-text>
          </div>
        </div>
      </ion-accordion>
    </ion-accordion-group>
  </ion-page>
</template>

<script lang="ts" setup>
/* Ionic components */
import { IonPage, IonAccordion, IonAccordionGroup, IonItem } from "@ionic/vue";
import { timeOutline } from "ionicons/icons";
</script>

<style scoped>
.waste-container {
  display: flex;
  align-items: center;
  justify-content: center;
}

.waste {
  height: 150px;
  width: 150px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.waste .icon {
  height: 100px;
  width: 100px;
  background-color: #eee;
  border: 1px solid #ddd;
  border-radius: 4px;
}

.waste .label {
  margin-top: 4px;
  text-align: center;
}

.footer {
  margin-top: 16px;
  display: flex;
  align-items: center;
}
.pl-8 {
  padding-left: 8px;
}
</style>
