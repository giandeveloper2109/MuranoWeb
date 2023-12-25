<template>
    <form @submit.prevent="submit">
      <v-text-field
        clearable
        v-model="name.value.value"
        :counter="10"
        :error-messages="name.errorMessage.value"
        label="Nombre"
      ></v-text-field>
  
      <v-text-field
        clearable
        v-model="phone.value.value"
        :counter="7"
        :error-messages="phone.errorMessage.value"
        label="Numero de celular"
      ></v-text-field>
  
      <v-text-field
        clearable
        v-model="email.value.value"
        :error-messages="email.errorMessage.value"
        label="Correo"
      ></v-text-field>
      
      
      <v-text-field
        clearable
        v-model="asunto.value.value"
        :counter="10"
        :error-messages="asunto.errorMessage.value"
        label="Asunto"
      ></v-text-field>      
      
    <!--
  
      <v-checkbox
        clearable
        v-model="checkbox.value.value"
        :error-messages="checkbox.errorMessage.value"
        value="1"
        label="Option"
        type="checkbox"
      ></v-checkbox>
    -->
      <v-btn
        class="me-4"
        type="submit"
      >
        submit
      </v-btn>
  
      <v-btn @click="handleReset">
        clear
      </v-btn>
    </form>
  </template>

<script setup>
  import { ref } from 'vue'
  import { useField, useForm } from 'vee-validate'

  const { handleSubmit, handleReset } = useForm({
    validationSchema: {
      name (value) {
        if (value?.length >= 2) return true

        return 'El nombre requiere mas de dos caracteres'
      },
      phone (value) {
        if (value?.length > 9 && /[0-9-]+/.test(value)) return true

        return 'El numero de celular requiere mas de 8 digitos'
      },
      email (value) {
        if (/^[a-z.-]+@[a-z.-]+\.[a-z]+$/i.test(value)) return true

        return 'Email invalido'
      },
      asunto (value) {
        if (value?.length >= 7) return true

        return 'El asunto debe tener mas de 6 digitos'
      },
      checkbox (value) {
        if (value === '1') return true

        return 'Debe ser revisado.'
      },
    },
  })
  const name = useField('name')
  const phone = useField('phone')
  const email = useField('email')
  const asunto = useField('asunto')
  const checkbox = useField('checkbox')



  const submit = handleSubmit(values => {
    alert(JSON.stringify(values, null, 2))
  })
</script>  
<style>
  .prepend-icon{
    color: rgb(255, 209, 3);
  }
</style>