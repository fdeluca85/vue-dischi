<template>
<div class="container">
    <div class="row">
        <div class="col" v-for="(album, index) in albums" :key="index">
           <AlbumCard :info="album"/>
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
    },
    data() {
        return{
            albums: null
        }
    },
    created() {
        axios.get('https://flynn.boolean.careers/exercises/api/array/music')
        .then((response) => {
            // handle success
            this.albums = response.data.response
            console.log(response.data.response);
        })
        .catch(function (error) {
            // handle error
            console.log(error);
        });

        }

}
</script>

<style lang='scss' scoped>

.row{
    display: flex;
    flex-wrap: wrap;
    .col{
        margin: 20px;
        background-color: #2E3A46;
        width: 200px;
        height: 400px;
        
    };

}
</style>