<template>
    <section class="introducing">
        <img src="../assets/vec.png" alt="" class="introducing__img-abs">
        <div class="container introducing__container">
            <h2 class="introducing__title">
                Introducing Superpeer Series
            </h2>
            <p class="introducing__text">With series, you can create and sell any combination of on-demand video and live stream content. With cohort-based classes you can interact with your audience in a more engaging way.</p>
            <img src="../assets/introducing.png" alt="" class="introducing__img">

            <div class="offer__items">
                <div class="offer__item">
                    <img src="../assets/offer1.png" alt="" class="offer__item-img">
                    <p class="offer__item-title">Engage with your audience</p>
                    <p class="offer__item-text">Connect with your subscribers through interactive livestreams, 1:1s, and our newest feature, Series.</p>
                </div>

                <div class="offer__item">
                    <img src="../assets/offer2.png" alt="" class="offer__item-img">
                    <p class="offer__item-title">Manage easier</p>
                    <p class="offer__item-text">We take care of scheduling, payments, and protecting your privacy, so that you don’t have to.</p>
                </div>

                <div class="offer__item">
                    <img src="../assets/offer3.png" alt="" class="offer__item-img">
                    <p class="offer__item-title">Earn, your way</p>
                    <p class="offer__item-text">Set your own rates and earn revenue through weekly livestreams, channel subscriptions, and even donations.</p>
                </div>
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "Introducing"
}
</script>

<style lang="scss">
.introducing {
    background: linear-gradient(180deg, #E4DDFF 0%, rgba(255, 255, 255, 0) 100%);
    position: relative;
    margin-top: 60px;
    padding-top: 80px;
    padding-bottom: 50px;
    &__container {
        text-align: center;
    }
    &__img-abs {
        width: 100%;
        position: absolute;
        top: -50px;
        right: 0;
        left: 0;
    }
    &__title {
        font-weight: bold;
        font-size: 48px;
        line-height: 53px;
        color: #222222;
        margin-bottom: 64px;
    }
    &__text {
        font-size: 18px;
        line-height: 25px;
        color: #222222;
        margin-bottom: 94px;
    }
    &__img {
        max-width: 870px;
        width: 100%;
        margin-bottom: 50px;
    }
}
@media only screen and (max-width: 750px) {
    .introducing {
        &__img-abs {
            top: -12px;
        }
        &__title {
            font-size: 28px;
            line-height: 34px;
        }
        &__text {
            font-size: 16px;
            line-height: 20px;
        }
    }
}
</style>