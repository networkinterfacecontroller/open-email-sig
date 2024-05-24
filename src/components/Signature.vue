<script setup>
import { form } from '../state/form.js'
import 'primeicons/primeicons.css'
import Card from 'primevue/card'
</script>

<template>
    <Card>
        <template #content>
            <table class="grid">
                <tr>
                <td class="col">
                    <img :src=form.imgurl height="100" />
                </td>

                <td class="col-8" style="padding-left: 20px; padding-top: 16px;">
                    {{ form.name }} <br />
                    <span v-if="form.role && form.company">
                        {{ form.role }} @ {{ form.company }}
                    </span> <br />
                    <a :href="form.website">{{ form.website }}</a>
                    <br /> <br />
                    <span style="padding-left: 3px;">
                        <span v-if="form.linkedin">
                            <a :href="form.linkedin"><img height="15" src="../assets/linkedin-in.png"></img></a>&nbsp;
                        </span>
                        <span v-if="form.instagram">
                            <a :href="form.instagram"><img height="15" src="../assets/instagram.png"></img></a>&nbsp;
                        </span>
                        <span v-if="form.facebook">
                            <a :href="form.facebook"><img height="15" src="../assets/facebook.png"></img></a>&nbsp;
                        </span>
                        <span v-if="form.twitter">
                            <a :href="form.twitter"><img height="15" src="../assets/x-twitter.png"/></a>&nbsp;
                        </span>
                    </span>
                    
                    <br />
                    {{ form.phone }}
                </td>
            </tr>
        </table>      
        </template>
    </Card>
</template>