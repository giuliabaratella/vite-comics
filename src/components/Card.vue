<template>
    <div class="card-comics">
        <div class="img-box mb-3">
            <img :src="img" :alt="title">
        </div>
        <h6 class="text-uppercase mb-5">{{title}}</h6>
    </div>
</template>

<script>
    export default {
        name:'Card',
        props: {
            img: String,
            title: String,
        }
    }
</script>

<style lang="scss" scoped>
.card-comics{
    width: 200px;
    .img-box{
        width: 200px;
        height: 200px;
        overflow: hidden;
        transition: all 0.1s;
        cursor: pointer;
    }
    &:hover{
        transform: scale(0.97);
    }
}
</style>
