<template>
    <main>
        <div class="main-section"></div>
        <div class="bonus-section"></div>
    </main>
</template>

<script>
export default{
        data() {
            return{
            }
        }
    }
</script>

<style lang="scss" scoped>

    .main-section{
        height: 130px;
        background-image:url(../assets/img/jumbotron.jpg);
        object-fit: scale-down;
    }

    .bonus-section{
        height: 150px;
        background-color: #0282F9;
    }
</style>