<template>
        <nav>
            <div class="nav-inner">
            <!--logo -->
            <div class="logo">
                <img src="../assets/images/logo.png" alt="">
            </div>
            <!--.limks -->
            <div class="links">
                <a href="#">About Us</a>
                <a href="#">Schmenken</a>
                <a href="#">Eliktronik</a>
                <a href="#">Kleidung</a>
                <a href="#">Mitglied Sein</a>
                <a href="#">Accessories</a>
                <a href="#">Kontakt</a>
            </div>
            <!-- icons-->
            <div class="icons">
               <span class="icon">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M21 21L15 15L21 21ZM17 10C17 10.9193 16.8189 11.8295 16.4672 12.6788C16.1154 13.5281 15.5998 14.2997 14.9497 14.9497C14.2997 15.5998 13.5281 16.1154 12.6788 16.4672C11.8295 16.8189 10.9193 17 10 17C9.08075 17 8.1705 16.8189 7.32122 16.4672C6.47194 16.1154 5.70026 15.5998 5.05025 14.9497C4.40024 14.2997 3.88463 13.5281 3.53284 12.6788C3.18106 11.8295 3 10.9193 3 10C3 8.14348 3.7375 6.36301 5.05025 5.05025C6.36301 3.7375 8.14348 3 10 3C11.8565 3 13.637 3.7375 14.9497 5.05025C16.2625 6.36301 17 8.14348 17 10Z" stroke="#121212" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
               </span> 
               <span class="icon">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M3.055 11H5C5.53043 11 6.03914 11.2107 6.41421 11.5858C6.78929 11.9609 7 12.4696 7 13V14C7 14.5304 7.21071 15.0391 7.58579 15.4142C7.96086 15.7893 8.46957 16 9 16C9.53043 16 10.0391 16.2107 10.4142 16.5858C10.7893 16.9609 11 17.4696 11 18V20.945M8 3.935V5.5C8 6.16304 8.26339 6.79893 8.73223 7.26777C9.20107 7.73661 9.83696 8 10.5 8H11C11.5304 8 12.0391 8.21071 12.4142 8.58579C12.7893 8.96086 13 9.46957 13 10C13 10.5304 13.2107 11.0391 13.5858 11.4142C13.9609 11.7893 14.4696 12 15 12C15.5304 12 16.0391 11.7893 16.4142 11.4142C16.7893 11.0391 17 10.5304 17 10C17 9.46957 17.2107 8.96086 17.5858 8.58579C17.9609 8.21071 18.4696 8 19 8H20.064M15 20.488V18C15 17.4696 15.2107 16.9609 15.5858 16.5858C15.9609 16.2107 16.4696 16 17 16H20.064L15 20.488ZM21 12C21 13.1819 20.7672 14.3522 20.3149 15.4442C19.8626 16.5361 19.1997 17.5282 18.364 18.364C17.5282 19.1997 16.5361 19.8626 15.4442 20.3149C14.3522 20.7672 13.1819 21 12 21C10.8181 21 9.64778 20.7672 8.55585 20.3149C7.46392 19.8626 6.47177 19.1997 5.63604 18.364C4.80031 17.5282 4.13738 16.5361 3.68508 15.4442C3.23279 14.3522 3 13.1819 3 12C3 9.61305 3.94821 7.32387 5.63604 5.63604C7.32387 3.94821 9.61305 3 12 3C14.3869 3 16.6761 3.94821 18.364 5.63604C20.0518 7.32387 21 9.61305 21 12Z" stroke="#121212" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

               </span>
               <span class="icon">
                <svg width="16" height="20" viewBox="0 0 16 20" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M12 5C12 6.06087 11.5786 7.07828 10.8284 7.82843C10.0783 8.57857 9.06087 9 8 9C6.93913 9 5.92172 8.57857 5.17157 7.82843C4.42143 7.07828 4 6.06087 4 5C4 3.93913 4.42143 2.92172 5.17157 2.17157C5.92172 1.42143 6.93913 1 8 1C9.06087 1 10.0783 1.42143 10.8284 2.17157C11.5786 2.92172 12 3.93913 12 5V5Z" stroke="#121212" stroke-linecap="round" stroke-linejoin="round"/>
<path d="M8 12C6.14348 12 4.36301 12.7375 3.05025 14.0503C1.7375 15.363 1 17.1435 1 19H15C15 17.1435 14.2625 15.363 12.9497 14.0503C11.637 12.7375 9.85652 12 8 12V12Z" stroke="#121212" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

        </span> 
        <span class="icon">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M16 11V7C16 5.93913 15.5786 4.92172 14.8284 4.17157C14.0783 3.42143 13.0609 3 12 3C10.9391 3 9.92172 3.42143 9.17157 4.17157C8.42143 4.92172 8 5.93913 8 7V11H16ZM5 9H19L20 21H4L5 9Z" stroke="#121212" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

        </span> 
        <span class="icon">
    
        </span>  
            </div>
        </div>
        </nav>
</template>

<script setup lang="ts">



</script>

<style scoped>
nav{
    border-bottom: 2px solid #f8f8f8;
}

nav .nav-inner{
    height: 90px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: calc(1440px - 170px);
    width: 100%;
    margin: auto;
}
.nav-inner .links a{
    margin:0px 16px;
    font-style:normal;
    font-weight:400;
    font-size:16px;
    line-height:1.25;
    color: #121212;
    border-bottom: 1px solid transparent;
    transition:.3s;
}
.nav-inner .links a:hover{
    border-color: black;
} 
.icons{
    display:flex;
    align-items: center;
}
.icons span{
    margin:0 13px;
    display:inline-block;
    display:flex;
    justify-content: center;
    align-items: center;
}
</style>