<template>
<div class="container">
    <div class="row">
        <div class="col">
           <AlbumCard />
        </div>
    </div>
</div>
  
</template>

<script>
import axios from 'axios';
import AlbumCard from "../commons/AlbumCard.vue"
export default {
    name: 'AlbumList',
    components:{
        AlbumCard
    }
}
</script>

<style>

</style>