<template>
    <ion-page>
        <ion-header>
            <ion-toolbar>
                <ion-title>Grid example</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
            <ion-grid>
                <ion-row>
                    <ion-col size="12" class="full">1 of 1</ion-col>
                </ion-row>
                <ion-row>
                    <ion-col size="6" size-xs="12" size-sm="12" size-md="12" size-lg="6" size-xl="6" class="mid">1 of 2</ion-col>
                    <ion-col size="6" class="mid2">2 of 2</ion-col>
                </ion-row>
            </ion-grid>
        </ion-content>
    </ion-page>
</template>
  
<script lang="ts" setup>
import { IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonCol, IonRow } from '@ionic/vue';
</script>
  
<style scoped>
    .full {
        background-color: blue;
    }
    .mid {
        background-color: red;
    }
    .mid2 {
        background-color: green;
    }
</style>
  