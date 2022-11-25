<template>
    <main>
        <div id="jumbotron">

        </div>
       <section id="products">
        <div class="container">
            <span class="etichetta">Current series</span>
            <!-- area fumetti -->
            <div class="area-fumetto">

                
                <!-- singolo fumetto ciclato -->
                <FumettoComp  
                 v-for="(elem, index) in fumetti" :key="index"
                 :datiFumetto="elem"/>

                
            </div>

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
                <img class="img-svg" src="../assets/img/buy-dc-power-visa.svg"  alt="">
                <span class="fs-small">DC POWER VISA</span>
            </div>
        </div>
       </section>
    </main>
</template>
  
<script>
import FumettoComp from '../components/FumettoComp.vue';

export default {
    name: 'MainComp',
    components: {
        FumettoComp
    },
    data() {
        return {
            fumetti: [
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
    "price": "$19.99",
    "series": "Action Comics",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
    "price": "$3.99",
    "series": "American Vampire 1976",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
    "price": "$16.99",
    "series": "Aquaman",
    "type": "graphic novel"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
    "price": "$2.99",
    "series": "Batgirl",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$3.99",
    "series": "Batman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
    "price": "$2.99",
    "series": "Batman Beyond",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
    "price": "$3.99",
    "series": "Batman/Superman",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
    "price": "$4.99",
    "series": "Batman/Superman Annual",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
    "price": "$5.99",
    "series": "Batman: The Joker War Zone",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
    "price": "$6.99",
    "series": "Batman: Three Jokers",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
    "price": "$4.99",
    "series": "Batman: White Knight Presents: Harley Quinn",
    "type": "comic book"
  },
  {
    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
    "price": "$16.99",
    "series": "Catwoman",
    "type": "graphic novel"
  }
            ]
        }
    },
}
</script>
  
<style scoped lang="scss">
@import '../style/variabili.scss';
#jumbotron{
    background-image: url('../assets/img/jumbotron.jpg');
    background-size: cover;
    background-repeat: no-repeat;
    min-height: 300px;
}


.container{
    margin: 0 auto;
    width: 80%;

    .etichetta{
        background-color: $bg-blue;
        padding: 10px;
        color: $text-light;
        position: relative;
        top: -38px;
    }

    .area-fumetto{
        display: flex;
        flex-wrap: wrap;

    }

    .fumetto{
        width: calc(100% / 6);
    }

    h5{
        width: 80%;
    }
}    


#dc-images>div,
#products>div{
    width: 80%;
    margin: 0 auto;
}
#dc-images{
    background-color: $bg-blue;
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 30px 0;

    div{
        gap: 10px;
        display: flex;
        align-items: center;
        justify-content: space-around;
        color: $text-light;
        font-weight: bold;

        img{
            height:50px;
        }

        .img-svg{
            width: 50px;
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