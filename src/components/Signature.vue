<script setup>
import { form } from '../state/form.js'
import 'primeicons/primeicons.css'
import Card from 'primevue/card'
</script>

<template>
    <Card>
        <template #content>      
            {{ form.name }} <br />
            {{ form.role }} @ {{ form.company }} <br />
            {{ form.website }} <br /> <br />
            <i class="pi pi-linkedin"></i>&nbsp;
            <i class="pi pi-instagram"></i>&nbsp;
            <i class="pi pi-facebook"></i>&nbsp;
            <i class="pi pi-twitter"></i>&nbsp; <br />
            {{ form.phone }}
        </template>
    </Card>
</template>