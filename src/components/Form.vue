<script setup>
import { reactive } from 'vue'
import InputText from 'primevue/inputtext'
import FieldSet from 'primevue/fieldset'
import Card from 'primevue/card'

import { form } from '../state/form.js'

</script>

<template>
    <Card>
        <template #content>
    <div class="flex justify-content-center">
        <div class="card p-fluid">
            <FieldSet legend="Who are you?" class="pt-1">
                <div class="field">
                    <label for="name" class="custom-float-label">Name</label>
                    <InputText id="name" v-model="form.name" />
                </div>
                <div class="field">
                    <label for="role" class="p-float-label">Role/Title</label>
                    <InputText id="role" v-model="form.role" />
                </div>
            </FieldSet>

            <FieldSet legend="Who do you work for?" class="pt-1">
                <div class="field">
                    <label for="company p-float-label">Company Name</label>
                    <InputText id="company" v-model="form.company" />
                </div>
                <div class="field">
                    <label for="imgurl">Logo URL</label>
                    <InputText id="imgurl" v-model="form.imgurl" />
                </div>
            </FieldSet>
            
            
            <FieldSet legend="Contact Info" class="pt-1">
                <div class="field">
                    <label for="phone">Phone</label>
                    <InputText id="phone" v-model="form.phone" />
                </div>
                <div class="field">
                    <label for="website">Website</label>
                    <InputText id="website" v-model="form.website" />
                </div>
            </FieldSet>
            
            <FieldSet legend="Socials" class="pt-1">
                <div class="field">
                    <label for="linkedin">LinkedIn</label>
                    <InputText id="linkedin" v-model="form.linkedin" />
                </div>
                <div class="field">
                    <label for="instagram">Instagram</label>
                    <InputText id="instagram" v-model="form.instagram" />
                </div>
                <div class="field">
                    <label for="facebook">Facebook</label>
                    <InputText id="facebook" v-model="form.facebook" />
                </div>
                <div class="field">
                    <label for="twitter">Twitter</label>
                    <InputText id="twitter" v-model="form.twitter" />
                </div>
            </FieldSet>
            
        </div>
    </div>

</template>
</Card>
   
</template>
