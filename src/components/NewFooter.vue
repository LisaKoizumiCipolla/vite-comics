<template>
    <footer>
        <div class="main-footer-container">

            <div class="main-footer wrapper">
                <div class="links flex">

                    <div>
                        <div>
                            <h2>DC COMICS</h2>
                            <ul class="link-list">
                                <li>Characters</li>
                                <li>Comics</li>
                                <li>Movies</li>
                                <li>TV</li>
                                <li>Games</li>
                                <li>Videos</li>
                                <li>News</li>
                            </ul>
                        </div>
                        <div>
                            <h2>SHOP</h2>
                            <ul class="link-list">
                                <li>Shop DC</li>
                                <li>Shop DC Collectibles</li>
                            </ul>
                        </div>
                    </div>

                    <div>
                        <h2>DC</h2>
                        <ul class="link-list">
                            <li>Terms Of Use</li>
                            <li>Privacy policy (New)</li>
                            <li>Ad Choices</li>
                            <li>Advertising</li>
                            <li>Jobs</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Ratings</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </div>

                    <div>
                        <h2>SITES</h2>
                        <ul class="link-list">
                            <li>DC</li>
                            <li>MAD Magazinbe</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </div>
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
                    <h2 class="follow">FOLLOW US</h2>
                    <ul class="flex logos">
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
        margin: 0 auto;
        @include flex(row, space-between, center);
        overflow: hidden;
        color: white;
    }

    h2{
        color: white;
        font-size: 1.35rem;
        font-weight: 700;
        margin-right: 5px;
        align-self: center;
    }

    .links{
        
    @include flex(row, start, flex-start);

        ul{
            margin: 20px 50px 20px 0;

            li{
            @include flex(column, start, flex-start);
            color: #797979;
            font-size: .85rem;
            line-height: 1.5;
            }
        }
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

    .logos{
        @include flex(row, center, center);

        li{
        color: #474747;
        border-radius: 50%;
        height: 30px;
        width: 30px;
        margin-left: 25px;
        }

    }

    .follow{
        color: #0282F9;
    }
</style>