<template>
    <ion-input :id="id" :value="value" :placeholder="placeholder" :clear-input="clearInput" :debounce="debounce" :disabled="disabled" :maxlength="maxlength" :min="min" :max="max" :step="step"></ion-input>
  </template>
  
  <script lang="ts">
  import { IonInput } from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    components: { IonInput },
    props: {
      id: {
        type: String,
        required: true
      },
      value: String,
      placeholder: String,
      clearInput: Boolean,
      debounce: Number,
      disabled: Boolean,
      maxlength: Number,
      min: Number,
      max: Number,
      step: Number
    }
  });
  </script>
  
  <style scoped>
  /* Estilos del componente */
  /* Estilos globales */
  </style>
  