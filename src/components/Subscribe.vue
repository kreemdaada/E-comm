<template>
    <section class="subscribe-section">
      <div class="subscribe-wrapper">
        <div class="img-container left">
          <img src="../assets/images/left.png" alt="" />
        </div>
        <div class="center-content">
          <h6>Special Angebot</h6>
          <h3>Subscribe und bekomme bis zu 10% Rabatt</h3>
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
    flex: 1; /* Grow to fill available space */
  }
  
  .subscribe-wrapper .center-content {
    flex: 2; /* Grow to fill more space than images */
    text-align: center;
  }
  
  .subscribe-wrapper .img-container img {
    max-width: 100%; /* Ensure images don't exceed their container width */
  }
  
  /* Adjust padding for the entire subscribe section */
  .subscribe-section {
    padding: 40px 0;
  }
  </style>
  