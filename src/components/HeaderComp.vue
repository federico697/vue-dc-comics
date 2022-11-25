<template>
    <header class="header">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li>
                <a href="#">CHARACTERS</a></li>
            <li>
                <a href="#">COMICS</a></li>
            <li>
                <a href="#">MOVIES</a></li>
            <li>
                <a href="#">TV</a></li>
            <LI>
                <a href="#">GAMES</a></LI>
            <LI>
                <a href="#">COLLECTIBLES</a></LI>
            <LI>
                <a href="#">VIDEOS</a></LI>
            <LI>
                <a href="#">FANS</a></LI>
            <LI>
                <a href="#">NEWS</a></LI>
            <LI>
                <a href="#">SHOP</a></LI>
        </ul>
    </header>
</template>
  
<script>
export default {
    name: 'HeaderComp'
}
</script>
  
<style scoped lang="scss">
@import '../style/variabili.scss';

header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 80%;
    margin: 0 auto;
}
ul{
    gap: 10px;
    display: flex;
    align-items: center;

    
    li{
        margin: 0 15px;
        font-size: 0.8rem;
        display: flex;
        align-items: center;



        a{
            color: #060606;
            align-self: center;
            padding: 60px 0;
            border-bottom: 3px solid $text-light;

            &:hover{
                color: $borders;
                border-bottom: 3px solid $borders;
            }
        }
    }
}

</style>
  