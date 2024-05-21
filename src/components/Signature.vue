<script setup>
import { form } from '../state/form.js'
import 'primeicons/primeicons.css'
import Card from 'primevue/card'
</script>

<template>
    <Card>
        <template #content>
            <div class="grid">
                <div class="col-2">

                </div>
                <div class="col-8">
                    {{ form.name }} <br />
                    {{ form.role }} @ {{ form.company }} <br />
                    {{ form.website }}
                    <br /> <br />
                    <i class="pi pi-linkedin"></i>&nbsp;
                    <i class="pi pi-instagram"></i>&nbsp;
                    <i class="pi pi-facebook"></i>&nbsp;
                    <i class="pi pi-twitter"></i>&nbsp; <br />
                    {{ form.phone }}
                </div>
            </div>      
        </template>
    </Card>
</template>