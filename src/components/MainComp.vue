<template>
    <main>
       <section id="products">
        <div>
            <h2>il contenuto andrà qui</h2>
        </div>
       </section> 
       <section id="dc-images">
        <div>
            <div class="flex">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                <span class="fs-small">DIGITAL COMICS</span>
            </div>
            <div class="flex">
                <img src="../assets/img/buy-comics-merchandise.png"  alt="">
                <span class="fs-small">DC MERCHANDISE</span>
            </div>
            <div class="flex">
                <img src="../assets/img/buy-comics-shop-locator.png"  alt="">
                <span class="fs-small">SUBSCRIPTION</span>
            </div>
            <div class="flex">
                <img src="../assets/img/buy-comics-subscriptions.png"  alt="">
                <span class="fs-small">COMICS SHOP LOCATOR</span>
            </div>
            <div class="flex">
                <img src="../assets/img/buy-dc-power-visa.svg"  alt="">
                <span class="fs-small">DC POWER VISA</span>
            </div>
        </div>
       </section>
    </main>
</template>
  
<script>
export default {
    name: 'MainComp'
}
</script>
  
<style scoped lang="scss">
#dc-images>div,
#products>div{
    width: 80%;
    margin: 0 auto;
}
#dc-images{
    background-color: rgb(49, 126, 235);
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 30px 0;
    color: white;

    div{
        display: flex;
        align-items: center;
        justify-content: space-around;

        img{
            height:50px;
        }
    }
}
.fs-small{
    font-size: 0.8rem;
    padding: 0 5px;
}
.flex{
    display: flex;
    justify-content: center;
    align-items: center;
}
#products{
    background-color: black;
    color: white;
    padding: 30px 0;
}
</style>