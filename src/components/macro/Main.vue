<template>
    <main>
        <AlbumList />
    </main>
  
</template>

<script>
import AlbumList from '../sections/AlbumList.vue'
export default {
    name: 'Main',
    components: {
        AlbumList
    }
}
</script>

<style lang='scss' scoped>
    main{
        background-color: #1E2D3B;
        height: 100vh;
    }


</style>