<template>
    <header>
        <div class="logo">
            <img src="../../assets/img/spotify_logo.png" alt="">

        </div>
    </header>
  
</template>

<script>
import logo from "../../assets/img/spotify_logo.png";
export default {
    name: 'Header',
    data() {
       return {
          image: logo
       }
    }
}
</script>

<style lang='scss' scoped>
    header{
        background-color: #2E3A46;
        height: 80px;
    }
    img{
        height: 50px;
        margin: 20px;
    }


</style>