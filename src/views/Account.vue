<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Cuenta</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Cuenta</ion-title>
        </ion-toolbar>
      </ion-header>

      <ExploreContainer :icon="person" name="Vista de Cuenta" />
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent, IonIcon } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';
import { person } from 'ionicons/icons';
</script>
