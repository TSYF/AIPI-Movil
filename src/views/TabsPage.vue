<template>
  <ion-page>
    <ion-tabs>
      <ion-router-outlet></ion-router-outlet>
      <ion-tab-bar slot="bottom">
        <ion-tab-button tab="home" href="/tabs/home">
          <ion-icon aria-hidden="true" :icon="homeOutline" />
          <ion-label>Inicio</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="search" href="/tabs/search">
          <ion-icon aria-hidden="true" :icon="search" />
          <ion-label>Buscar</ion-label>
        </ion-tab-button>

        <ion-tab-button
          tab="speak"
          href="/tabs/speak"
          style="
            position: sticky;
            transform: translateY(-1.2rem);
          "
        >
          <ion-icon
            aria-hidden="true"
            :icon="mic"
            style="
              font-size: xx-large;
              outline: 1px solid #FFFF;
              border-radius: 2em;
              padding: .2em;
            "
          />
        </ion-tab-button>

        <ion-tab-button tab="reports" href="/tabs/reports">
          <ion-icon aria-hidden="true" :icon="barChart" />
          <ion-label>Reportes</ion-label>
        </ion-tab-button>

        <ion-tab-button tab="account" href="/tabs/account">
          <ion-icon aria-hidden="true" :icon="personOutline" />
          <ion-label>Cuenta</ion-label>
        </ion-tab-button>
      </ion-tab-bar>
    </ion-tabs>
  </ion-page>
</template>

<script setup lang="ts">
import { IonTabBar, IonTabButton, IonTabs, IonLabel, IonIcon, IonPage, IonRouterOutlet } from '@ionic/vue';
import { barChart, homeOutline, mic, personOutline, search } from 'ionicons/icons';
</script>
