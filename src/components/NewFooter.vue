<template>
    <footer>
        <div class="main-footer-container">

            <div class="main-footer wrapper">
                <div class="links">
                    blablabla
                </div>
                <div class="logo">
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </div>
            </div>

        </div>

        <div class="contacts-container">
            <div class="contacts wrapper">
                <div class="button">SIGN-UP NOW!</div>
                <nav>
                    lgjrlkgjlgam

                </nav>
            </div>
        </div>
    </footer>
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

    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    .main-footer-container{
        height: 370px;
        background-image: url(../assets/img/footer-bg.jpg);
        background-size: cover;
    }
    .main-footer{
        height: 100%;
        margin: auto;
        @include flex(row, space-between, center);
        overflow: hidden;
        color: white;
    }

    .contacts-container{
        background-color: #303030;
        height: 110px;  
        @include flex(row, center, center);
    }

    .contacts{
        margin: auto;
        @include flex(row, space-between, center);
    }

    .button{
        background-color: #303030;
        color: white;
        border: 2px solid #0282F9;
        padding: 15px;
        font-weight: 600;
    }
</style>