<template>
<section class="featured-products">
   <div class="container">
    <div class="products">
    <div class="product">
    <div class="img-container">
        <img src="../assets/images/f1.jpg" alt="" />
        <div class="content">
            <h6>New Season</h6>
            <h3>New collection</h3>
            </div>
          </div>
         </div>
         <div class="product">
          <div class="img-container">
           <img src="../assets/images/f2.jpg" alt="" />
              <div class="content">
            <h6>New Season</h6>
            <h3> bis <span> 50% Rabatt</span></h3>
            </div>
          </div>
         </div>
     </div>
 </div> 
</section>
</template>


<script setup>

</script>


<style scoped>
.featured-products {
    margin-bottom:50px;
}

.products{
    display: grid;
    grid-template-columns:1fr 1fr;
    gap:30px;
}
.products img{
    object-fit: cover;
    padding:88px;
}
.products .img-container{
    position: relative;
}
.products .content{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translateY(-50%, -50%);
    padding: 16px;
    background-color:#fff;
    text-align:center;
}   
.content h6{
    font-weight:600;
    font-size:12px;
    line-height:13px;
    margin-bottom:6px;
    opacity:0,6;
}
.content h3{
    font-weight:600;
    font-size:16px;
    line-height:18px;
    text-transform:uppercase;
}
.content h3 span{
    color: #E91E63;

}
</style>