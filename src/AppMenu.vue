<template>
    <ion-menu content-id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-title>Menu Example</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
            <p> Hello world</p>
        </ion-content>
    </ion-menu>
    <ion-page id="main-content">
        <ion-header>
            <ion-toolbar>
                <ion-buttons slot="start">
                    <ion-menu-button></ion-menu-button>
                </ion-buttons>
                <ion-title>App Menu</ion-title>
            </ion-toolbar>
        </ion-header>
        <ion-content class="ion-padding">
            Tab to open
        </ion-content>
    </ion-page>
</template>
  
<script lang="ts" setup>
import { IonMenu, IonHeader, IonToolbar, IonTitle, IonContent, IonPage, IonButtons, IonMenuButton } from '@ionic/vue';
</script>
  
<style scoped>
</style>
  