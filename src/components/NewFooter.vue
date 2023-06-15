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
                    <h2>FOLLOW US</h2>
                    <ul class="flex">
                        <li>
                            <img src="../assets/img/footer-facebook.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-twitter.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-youtube.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-pinterest.png" alt="">
                        </li>
                        <li>
                            <img src="../assets/img/footer-periscope.png" alt="">
                        </li>
                    </ul>
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
        font-weight: 500;

        &:hover{
            cursor: pointer;
            background-color: #474747;
        }
    }

    nav{
        display: flex;
    }

    ul{
        @include flex(row, center, center);
    }

    li{
        color: #474747;
        border-radius: 50%;
        height: 30px;
        width: 30px;
        margin-left: 25px;
    }

    h2{
        color: #0282F9;
        font-size: 1.35rem;
        font-weight: 700;
        margin-right: 5px;
        align-self: center;
    }
</style>