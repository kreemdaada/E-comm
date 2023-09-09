<template>
    <section class="subscribe-section">
      <div class="subscribe-wrapper">
        <div class="img-container left">
          <img src="../assets/images/left.png" alt="" />
        </div>
        <div class="center-content">
          <h6>Special Angebot</h6>
          <h3>Subscribe und bekomme<span> bis zu 10% Rabatt</span></h3>
          <input type="text" placeholder="Enter your email">
          <button class="btn">Subscribe</button>
        </div>
        <div class="img-container right">
          <img src="../assets/images/right.png" alt="" />
        </div>
      </div>
    </section>
  </template>
  
  <script setup>
  </script>
  
  <style scoped>
  section {
    background: linear-gradient(100deg, #f3f2f2, #dcdbdb 100%);
    padding: 60px 0px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  
  .subscribe-wrapper {
    max-width: 532px;
    width: 100%;
    margin: auto;
    background: #fff;
    position: relative;
    display: flex;
    align-items: center;
  }
  
  .subscribe-wrapper .img-container {
    flex: 1; 
  }
  
  .subscribe-wrapper {
    flex: 2;
    text-align: center;
  }
  
  .subscribe-wrapper .img-container img {
    max-width: 100%; 
  }
  

  .subscribe-section {
    padding: 40px 0;
  }
  .subscribe-wrapper h6{
    font-size: 12px;
    font-weight: 600;
    line-height: 13px;
    opacity:0.4;
  }
  .subscribe-wrapper h3 {
    font-size: 29px;
    font-weight: 700;
    line-height: 36px;
    max-width: 300px;
    text-align: center;
    margin:auto;

  }
  .subscribe-wrapper h3 span {
    color:#e91e63;
  }
  input {
    height:64px;
    max-width:340px;
    margin:auto;
    background : #f8f8f8;
    text-align: center;
    border:none;
    outline: none;
    width:100%;
    margin-bottom:20px;
  }
  .subscribe-wrapper .btn{
    max-width:340px;
    height:64px;
    background : #121212;
    margin:auto;
    font-size:16px;
    line-height:18px;
    text-transform: uppercase;
    color:#ffffff;
    opacity:0.9;
    border:4px solid #121212;
    font-weight:500;
  }
  
  </style>

  