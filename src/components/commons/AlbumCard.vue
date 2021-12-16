<template>
<div class="album">
    <img :src="info.poster" alt="">
    <h2>{{info.title}}</h2>
    <h3>{{info.author}}</h3>
    <h3>{{info.year}}</h3>
</div>
  
</template>

<script>
export default {
    name: 'AlbumCard',
    props: {
        info: Object
    }

}
</script>

<style>

</style>