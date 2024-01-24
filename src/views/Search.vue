<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>Buscar</ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large">Buscar</ion-title>
        </ion-toolbar>
      </ion-header>

      <ExploreContainer :icon="search" name="Vista de Buscar" />
    </ion-content>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent } from '@ionic/vue';
import ExploreContainer from '@/components/ExploreContainer.vue';
import { search } from 'ionicons/icons';
</script>
