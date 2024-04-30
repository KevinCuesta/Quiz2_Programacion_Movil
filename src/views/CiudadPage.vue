<template>
    <ion-page>
    <ion-header :translucent="true">
        <ion-toolbar>
        <ion-title>Ciudad</ion-title>
        </ion-toolbar>
    </ion-header>  
    <ion-content>       
        <div id="login-container">  
        <div id="login-form">
            <LugarComponent id="id" name="id" type="text"/>
            <LugarComponent id="codigo" name="codigo" label="Código Dane: " />
            <LugarComponent id="nombre" name="nombre" label="Nombre: " />
        </div>
        <div> 
            <CrudButtonComponent />
        </div>         
        </div>
    </ion-content>
    </ion-page>
</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import LugarComponent from '@/components/LugarComponent.vue';
import CrudButtonComponent from '@/components/CrudButtonComponent.vue';
</script>

<style scoped src="../theme/container.css"></style>
