<template>
  <div class="banner"> 
     <div class="container">
       <div class="banner-content">
        <div class="main-banner">
         <div class="img-container">
           <img src="../assets/images/bild1.jpg" alt="" />
           <div class="img-content">
           <span>Banner</span>
           <h3>Dein text</h3>
            </div>
         </div>
       </div>
       
       <div class="category-banner">    
       <div class="top">
         <div class="img-container">
           <img src="../assets/images/bild2.png" alt="" />
           <div class="img-content">
           <span>Frau</span>
           <h3>Dein text</h3>
            </div>
         </div>
         <div class="img-container">
           <img src="../assets/images/bild3.png" alt="" />
           <div class="img-content">
           <span>Mann</span>
           <h3>Dein text</h3>
          </div>
         </div>
        </div>
       </div>
      </div>
      <div class="banner-sevieces">
        <div v-for="n in 3" :key="n" class="service">
          <span class="icon">
            <svg width="40" height="40" viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
            <g opacity="0.8">
            <path d="M21.6667 26.6667V10C21.6667 9.55801 21.4911 9.13409 21.1785 8.82153C20.8659 8.50897 20.442 8.33337 20 8.33337H6.66667C6.22464 8.33337 5.80072 8.50897 5.48816 8.82153C5.17559 9.13409 5 9.55801 5 10V26.6667C5 27.1087 5.17559 27.5327 5.48816 27.8452C5.80072 28.1578 6.22464 28.3334 6.66667 28.3334H8.33333M21.6667 26.6667C21.6667 27.1087 21.4911 27.5327 21.1785 27.8452C20.8659 28.1578 20.442 28.3334 20 28.3334H15M21.6667 26.6667V13.3334C21.6667 12.8913 21.8423 12.4674 22.1548 12.1549C22.4674 11.8423 22.8913 11.6667 23.3333 11.6667H27.6433C28.0853 11.6668 28.5092 11.8425 28.8217 12.155L34.5117 17.845C34.8242 18.1575 34.9999 18.5814 35 19.0234V26.6667C35 27.1087 34.8244 27.5327 34.5118 27.8452C34.1993 28.1578 33.7754 28.3334 33.3333 28.3334H31.6667M21.6667 26.6667C21.6667 27.1087 21.8423 27.5327 22.1548 27.8452C22.4674 28.1578 22.8913 28.3334 23.3333 28.3334H25M8.33333 28.3334C8.33333 29.2174 8.68452 30.0653 9.30964 30.6904C9.93477 31.3155 10.7826 31.6667 11.6667 31.6667C12.5507 31.6667 13.3986 31.3155 14.0237 30.6904C14.6488 30.0653 15 29.2174 15 28.3334M8.33333 28.3334C8.33333 27.4493 8.68452 26.6015 9.30964 25.9764C9.93477 25.3512 10.7826 25 11.6667 25C12.5507 25 13.3986 25.3512 14.0237 25.9764C14.6488 26.6015 15 27.4493 15 28.3334M31.6667 28.3334C31.6667 29.2174 31.3155 30.0653 30.6904 30.6904C30.0652 31.3155 29.2174 31.6667 28.3333 31.6667C27.4493 31.6667 26.6014 31.3155 25.9763 30.6904C25.3512 30.0653 25 29.2174 25 28.3334M31.6667 28.3334C31.6667 27.4493 31.3155 26.6015 30.6904 25.9764C30.0652 25.3512 29.2174 25 28.3333 25C27.4493 25 26.6014 25.3512 25.9763 25.9764C25.3512 26.6015 25 27.4493 25 28.3334" stroke="#121212" stroke-linecap="round" stroke-linejoin="round"/>
            </g>
            </svg>
          </span>
          <div class="details">
            <h6>FREE SHIPING</h6>
            <p>Order für 100$ bekommen Sie ein geschicnk umsonst</p>
          </div>
        </div>
      </div>
     </div>
    </div>
        
</template>

<script setup lang="ts">

</script>

<style scoped>
img{
 height: 100%;
}
.banner{
  border-bottom: 2px solid #f8f8f8;
  margin-bottom:100px;
}
.banner .container{
 max-width : calc(1440px - 170px);
 width: 100%;
 margin:auto;
}
.banner-content{
 display: flex;
 justify-content: space-between;
 padding: 40px 0px;
}
 .banner-content > div{
   flex :0 0 calc(50%-20px);
   max-width: 0 0 calc(50%-20px);
   width:100%;
   
 }

.img-container{
 position:relative;
 height:90%;
 width:90%;
}
.img-container img{
width:80%;
object-fit:cover;
}
.img-container .img-content{
 position:absolute;
 top:50%;
 left:50%;
 transform:translate(-50%,-50%);
 background:#ffffff;
 border-radius:4px;
 padding:16px 23px;
 text-align:center;
}
.img-content span{
 font-weight:600;
 font-size:12px;
 line-height:13px;
 color:#121212;
 opacity:0.4;
}
.img-content h3{
 font-weight:600;
 font-size:22px;
 line-height:25px;
 color:#121212;
 text-transform:uppercase;
 margin-top:5px;
}
.category-banner .top{
 display:flex;
 justify-content:space-between;
 margin-bottom:30px;
}
.category-banner .top > div{
   flex :0 0 calc(50% - 20px);
   max-width: calc(50% - 20px);
   width:100%;
}
.banner-sevieces{
  display:flex;
  justify-content:space-between;
  margin-bottom:30px;
}
.banner-sevieces > div{
   flex :0 0 calc(33.3% - 20px);
   max-width: calc(33.3% - 20px);
   width:100%;
   display:flex;
   align-items:center;
}
.service {
  margin-left:10px;
}
.details h6{
font-weight:600;
font-size:12px;
line-height:12px;
}
.details p{
  font-weight:500;
  font-size:12px;
  line-height:22px;
  opacity:0.9;
}
</style>
