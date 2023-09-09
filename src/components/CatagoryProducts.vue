<template>
    <section class="catagory-products">
    <div class="container">
      <CatagoryHeader :title="title" :tabs="tabs" />  
             <div class="products">
                <SingleProduct
                v-for ="(product,i) in products"
                :key="i"
                :product="product"
                />
            </div>  
            <button class="btn">Zeig Alles</button> 
    </div>
    
</section> 
</template>

<script setup>
import {defineProps}from 'vue';
import CatagoryHeader from "./CatagoryHeader.vue"
import SingleProduct from "./SingleProduct.vue"

defineProps (["title","products","tabs"])
</script>

<style scoped>

.container{
 max-width : calc(1440px - 170px);
 width: 100%;
 margin:auto;
}

.catagory-products{
    margin-bottom:100px;
}
.catagory-products .btn{
    height: 48px !important;
  background: #f8f8f8 !important;
  border: 2px solid #f8f8f8 !important;
  width:100%;
    margin-top:98px;
}

.products{
    display:grid;
    grid-template-columns:1fr 1fr 1fr 1fr;
    gap:30px;
}
</style>