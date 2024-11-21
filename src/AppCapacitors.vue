<template>
    <ion-page>
            <ion-header>
                <ion-toolbar>
                    <ion-title>Capacitor example</ion-title>
                </ion-toolbar>
            </ion-header>
            <ion-content class="ion-padding">
                <img :src="imageURL" />
                <button @click="makePhoto">Make photo</button>
            </ion-content>
    </ion-page>
</template>
  
<script lang="ts" setup>
    import { IonHeader, IonToolbar, IonTitle, IonContent, IonPage } from '@ionic/vue';
    import {Camera, CameraResultType} from '@capacitor/camera';
    import {ref} from 'vue';

    const imageURL = ref()

    const makePhoto = async () => {
        const image = await Camera.getPhoto({
            quality: 80,
            allowEditing: true,
            resultType: CameraResultType.Uri
        });
        imageURL.value = image.webPath;
        console.log(image);
    }


</script>
  
<style scoped>
</style>
  