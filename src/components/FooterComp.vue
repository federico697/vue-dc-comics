<template>
    <div>
        <footer>
            <div class="container">
                <div class="footer-lists">
                    <ul>
                        <li>ciao</li>
                    </ul>
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
    height: 300px;
    color: white;
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
.container{
    margin: 0 auto;
    width: 80%;
    display: flex;
    justify-content: space-between;
}
.w-80{
    display: flex;
    justify-content: space-between;
    width: 80%;
    margin: 0 auto;
}
</style>