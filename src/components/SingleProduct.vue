<template>
                <div class="single-product">
                    <div class="img-container">
                    <img :src= "product.img" alt="" />
                    <div v-if="product.sale" class="sale">-50%</div>
                    </div>
                    <div class="product-content">
                        <h6 class="name">Short sleeved Hoodi</h6>
                        {{ product.name }}
                        <div class="bewertung">
                            <span class="price">$32.55</span>
                            {{ product.price }}
                            <span class="icon">
                                <img :src= "product.bewertung" alt="" >
                            </span>
                        </div>
                    </div>
                </div>
</template>

<script setup>
import {defineProps} from "vue";
 
defineProps({
    product:{
        type: Object,
    },
});
</script>

<style scoped>
.singel-product .img-container{
    position:relative;
}
.singel-product .img-container .sale{
    position:absolute;
    top:0;
    left:0;
    padding:9;
    background:red;
    right: auto;
}
.single-product  .product-content h6{

    padding: 10px 0px;
}
.single-product  .product-content h6{
    font-size:14px;
    font-weight:400;
    line-height:16px;
    opacity:0.6;
}
.single-product .product-content .bewertung{
    display:flex;
    justify-content:space-between; 
    align-items:center;
    margin-top:5px;
    
}
.single-product .bewertung .price{
    font-weight:700;
    font-size:12px;
    line-height:16px;  
}

</style>