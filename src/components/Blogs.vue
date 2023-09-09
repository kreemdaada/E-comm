<template>
<sction class="blogs">
    <div class="container">
        <div class="blogs-header">
         <h3>ENDE VON BLOG</h3>
         <a href="#">Zeig Alles</a>   
        </div>
        <div class="blogs-wapper">
            <div class="blog">
                <div class="img-container">
                    <img src="../assets/images/blog3.jpg" alt="" />
                </div>
                <div class="blog-content">
                    <h3>
                        Die einfacher weg zum Kaufen</h3>
                    <p>
                        But I must explain to you how all 
                        idea of denouncing pleas and praising 
                    </p>
                </div>
            </div>
            <div class="blog">
                <div class="img-container">
                    <img src="../assets/images/blog2.jpg" alt="" />
                </div>
                <div class="blog-content">
                    <h3>
                        Die einfacher weg zum Kaufen</h3>
                    <p>
                        But I must explain to you how all 
                        idea of denouncing pleas and praising 
                    </p>
                </div>
            </div>
            <div class="blog">
                <div class="img-container">
                    <img src="../assets/images/blog1.jpg" alt="" />
                </div>
                <div class="blog-content">
                    <h3>
                        Die einfacher weg zum Kaufen</h3>
                    <p>
                        But I must explain to you how all 
                        idea of denouncing pleas and praising 
                    </p>
                </div>
            </div>
        </div>
    </div>
</sction>
</template>


<style scoped>
.blogs .blogs-header{
    justify-content:space-between;
    text-align:center;
    display:flex;
    margin-bottom:48px;
}
.blogs-header h3{
    font-weight:600;
    font-size:22px;
    line-height:25px;
    margin-left:80px;
    margin-top:30px;
}

.blogs-header a{
    font-weight:500;
    font-size:12px;
    line-height:13px;
    color:#121212;
    opacity:0.6;
    margin-right:80px;
    margin-top:30px;
}
.blogs-wapper{
    display:flex;
    grid-template-columns:1fr 1fr 1fr;
    gap:30px;
    margin-left:60px;
}
.blog .blog-content{
    max-width:calc(100% -48px);
    width:100%;
    margin:auto;
    transform:translateY(-100px);
    background-color: #fff;
    padding:24px 16px;
}
 .blog{
    margin-left:20px;

}

</style>