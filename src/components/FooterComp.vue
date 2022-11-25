<template>
    <div>
        <footer>
            <div class="container">
                <div class="footer-lists">
                    <!-- liste menu -->
                    <div>
                        <h3>DC COMICS</h3>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li><a href="#">News</a></li>
                        </ul>
                        <h3>SHOP</h3>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                    <div>
                        <h3>DC</h3>
                        <ul>
                            <li><a href="#">Terme Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Terme Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                        </ul>
                    </div>
                    <div>
                        <h3>SITES</h3>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>
                <div class="dc-logo-bg">

                </div>
            </div>
        </footer>
        <section>
            <div class="w-80">
                <button>SING-UP NOW!</button>
                <div class="flex">
                    <div>FOLLOW US</div>
                    <div><img src="../assets/img/footer-facebook.png" alt=""></div>
                    <div><img src="../assets/img/footer-periscope.png" alt=""></div>
                    <div><img src="../assets/img/footer-pinterest.png" alt=""></div>
                    <div><img src="../assets/img/footer-twitter.png" alt=""></div>
                    <div><img src="../assets/img/footer-youtube.png" alt=""></div>
                </div>
            </div>
        </section>
    </div>

</template>
  
<script>
export default {
    name: 'FooterComp'
}
</script>
  
<style scoped lang="scss">
footer{
    background-image: url('../assets/img/footer-bg.jpg');
    background-position: center;
    background-repeat: no repeat;
    background-size: cover;

    .container{
        margin: 0 auto;
        width: 80%;
        display: flex;
        justify-content: space-between;
    }

    .footer-lists{
        padding: 30px 0;
        display: flex;
        gap: 10px;

        ul{
            font-size: 14px;
        }
        a{
            color: rgb(158, 152, 152);
        }
    }

    h3{
        color: white;
    }

    .dc-logo-bg{
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        width: 40%;
    }
}


.w-80{
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: 0 auto;
}
section{
    background-color: rgb(60, 60, 60);
}
button{
    margin: 20px 0;
}
.flex{
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 40%;
}
</style>