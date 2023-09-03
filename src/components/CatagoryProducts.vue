<template>
    <div>
    <div class="container">
      <div class="catagory-header">
        <h3>FRAUEN</h3>
        <div class="tabs">
            <div
             v-for="( tab,i ) in tabs"
             :key="tab"
             class="tab"
             @click="activeIndex = i"
             :class="{ active :activeIndex === i }"
             >
             {{ tab }}
             </div>
             </div>
            </div>
             <div class="products">
                <SingleProduct
                v-for ="(product,i) in products"
                :key="i"
                :product="product"
                />
                <div class="single-product">
                    <div class="img-container">
                    <img src= "../assets/images/b1.png" alt="" />
                    <div class="sale">-50%</div>
                    </div>
                    <div class="product-content">
                        <h6 class="name">Short sleeved Hoodi</h6>
                        <div class="bewertung">
                            <span class="price">$32.55</span>
                            <span class="icon">
                                <img src= "../assets/images/bewertung.png" alt="" >
                            </span>
                        </div>
                    </div>
                </div>
            </div>
            <button class="btn">Zeig Alles</button>
    </div>
</div>
</template>

<script setup>
import {ref}from 'vue';
import SingleProduct from "./SingleProduct.vue"

const tabs = ref ([
    "Neue SACHEN",
    "SPIEZEALL",
    "BESTSELLERS",
    "MOST VIEWED",
    "FEATURED PROUDUCTS",
])
const activeIndex = ref(0)
const products=ref([
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
</script>

<style scoped>

.container{
max-width:calc(1440px - 170px);
width:100%;
margin:auto;
}
 .tab{
    background-color:transparent;
    border:none;
    transition:.3s;
    cursor:pointer;
    width:100%;
    display:flex;
    justify-content:center;
    align-items:center;
 }
.catagory-header{
    display:flex;
    justify-content:space-between;
    align-items:center;
    margin-bottom:50px;
}
.catagory-header h3{
    font-style:normal;
    font-weight:600;
    font-size:22px;
    line-height:25px;
}
.tabs{
    display:flex;
    align-items:center;
    flex :0.7;
    justify-content:flex-end;
}
.tabs .tab{
    font-weight:500;
    font-size:12px;
    line-height:13px;
    opacity:0.6;
    transition:.3s;
    margin-right:32px;
    cursor:pointer;
}
.tabs .tab.active,
.tabs .tab:hover
{
    opacity:1;
}
.products{
    display:grid;
    grid-template-columns:1fr 1fr 1fr 1fr;
    gap:30px;
}
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