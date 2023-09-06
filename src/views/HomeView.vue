<script setup lang="ts">
import BannerView from "../components/BannerView.vue"
import CatagoryProducts from "../components/CatagoryProducts.vue"
import {ref} from "vue"
import Featured from "../components/Featured.vue"
import Subscribe from "../components/Subscribe.vue"
const Frauentabs = ref ([
    "Neue SACHEN",
    "SPIEZEALL",
    "BESTSELLERS",
    "MOST VIEWED",
    "FEATURED PROUDUCTS",
])

const Frauenproducts=ref([
    {
        img:'../src/assets/images/b1.png',
        sale: true,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png"
    },
    {
        img:'../src/assets/images/b2.png',
        sale: true,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png" 
    },
    {
        img:'../src/assets/images/b3.png',
        sale:false,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png"
    },
    {
        img:'../src/assets/images/b1.png',
        sale: false,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png"
    },
    {
        img:'../src/assets/images/b2.png',
        sale: false,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png" 
    },
    {
        img:'../src/assets/images/b3.png',
        sale:false,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png"
    }, 
    {
        img:'../src/assets/images/b2.png',
        sale: false,
        name: `Short sleeved Hoodi`,
        price: "$32.55",
        bewertung:"../src/assets/images/bewertung.png"
    }

])
const Frauentitle = ref('Frauen')
const Mantitle = ref('Man')

</script>

<template>
<div>
    <BannerView />
    <CatagoryProducts 
    :tabs="Frauentabs" 
    :title="Frauentitle"
    :products="Frauenproducts"
    />
    <CatagoryProducts 
    :tabs="Frauentabs" 
    :title="Mantitle"
    :products="Frauenproducts"
    />
    <Featured/>
    <Subscribe/>
</div>
</template>


<style scoped>

</style>


