<template>
    <header class="header">
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li>
                <a href="#">CHARACTERS</a></li>
            <li>
                <a class="active-a" href="#">COMICS</a></li>
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
        list-style-type: none;
        margin: 0 15px;
        font-size: 0.8rem;
        display: flex;
        align-items: center;



        a{
            color: #060606;
            text-decoration: none;
            align-self: center;
            padding: 60px 0;
        }
    }

    .active-a{
        color: #0282f9;
        border-bottom: 3px solid #0282f9;
    }

}

</style>
  