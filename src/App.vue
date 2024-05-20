<script setup>
import Form from './components/Form.vue'
import Signature from './components/Signature.vue'
import Settings from './components/Settings.vue'

</script>

<template>
  <div class="grid justify-content-center">
    <div class="col-4 m-3">
      <Form />
    </div>
    <div class="col-4 m-3">
      <Settings class="mb-3"/>
      <Signature />
    </div>   
  </div>
</template>

<style>

</style>

