<template>
    <div class="product-wrapper">
        <div class="single-img">
            <img :src="comicElement.thumb" alt="">
        </div>
        <h4>
            {{ comicElement.series }}
        </h4>
    </div>
</template>
<script>
export default {
    props:{
        comicElement : Object
    },
}
</script>
<style lang="scss" scoped>
    .product-wrapper{
        width: calc((100% / 6) - 20px);
        background-color: #1c1c1c;
        padding-top: 30px;

        img{
            width: 100%;
        }

        &:hover{
                cursor: pointer;
        }
    }

    .single-img{
            height: 200px;
            overflow: hidden;
    }

    h4{
        font-weight: 400;
        padding-top: 20px;
        padding-bottom: 20px;
    }
</style>