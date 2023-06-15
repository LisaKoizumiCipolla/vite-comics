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

<style lang="scss">

    .main-section{
        height: 140px;
        background-image:url(../assets/img/jumbotron.jpg);
        object-fit: scale-down;
    }

    .bonus-section{
        height: 160px;
        background-color: #0282F9;
    }
</style>