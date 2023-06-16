<template>
    <main>
        <div class="jumbotron">

        </div>

        <div class="main-section">
            <div class="wrapper">
                <div class="square label">
                    CURRENT SERIES
                </div>
                    <ComicsList />
                <div class="square button">
                    LOAD MORE
                </div>
            </div>
        </div>

        <div class="bonus-section flex">
            <div class="wrapper">
                <ul class="flex">
                    <li>
                        <img src="../assets/img/buy-comics-digital-comics.png" alt="">
                        <span>DIGITAL COMICS</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-merchandise.png" alt="">
                        <span>DC MERCHANDISE</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-subscriptions.png" alt="">
                        <span>SUBSCRIPTION</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy-comics-shop-locator.png" alt="">
                        <span>COMIC SHOP LOCATOR</span>
                    </li>
                    <li>
                        <img class="svg" src="../assets/img/buy-dc-power-visa.svg" alt="">
                        <span>DC POWER VISA</span>
                    </li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>
import ComicsList from './ComicsList.vue'

export default{
        data() {
            return{
            }
        },

        components : {
            ComicsList
        }
    }
</script>

<style lang="scss" scoped>

    @use '../styles/partials/mixins' as *;
    @use '../styles/partials/variables' as *;
    .jumbotron{
        height: 400px;
        background-image:url(../assets/img/jumbotron.jpg);
        object-fit: scale-down;
    }

    .main-section {
        position: relative;
        background-color: #1c1c1c;
        color: white;
        padding: 25px 0 20px;
    }

    .bonus-section{
        height: 150px;
        background-color: #0282F9;
        @include flex(row, center, center);
    }

    .wrapper{
        margin: auto;
    }

    .square{
        background-color: #0282F9;
        color: white;
        font-weight: 700;
    }

    .label{
        position: absolute;
        font-size: 1.75rem;
        padding: 10px 25px;
        top: -28px;
        left: 310px;
    }

    .button{
        margin: 0 auto;
        width: 190px;
        text-align: center;
        padding: 10px 50px;
        font-size: .9rem;
        margin-top: 20px;

        &:hover{
            cursor: pointer;
        }
    }

    ul{
    @include flex(row, space-around, center);

        li{
            display: flex;
            align-items: center;
            color: white;
            font-size: .95rem;
            font-weight: 400;

            img{
                height: 55px;
                margin-right: 20px;
            }

            .svg{
                height: 35px;
            }

            &:hover{
                        cursor: pointer;
            }
        }
    }
</style>