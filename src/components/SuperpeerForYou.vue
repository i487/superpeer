<template>
    <section class="offer">
        <img src="../assets/offer.png" alt="" class="offer__img">
        <div class="container offer__container">
            <h2 class="offer__title">What can Superpeer do for you?</h2>
            <p class="offer__text">Turn your audience into loyal, paying followers with our seamless video experience and subscriber management tools.</p>

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

            <button class="features">All Features
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M19.5 16.25L23.25 12.5L19.5 8.75M23.25 12.5H0.75H23.25Z" stroke="#222222" stroke-width="0.0625" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
            </button>
        </div>
    </section>
</template>

<script>
export default {
    name: "SuperpeerForYou",
}
</script>

<style lang="scss">
.offer {
    padding-top: 100px;
    padding-bottom: 100px;
    background: linear-gradient(180deg, #FDE6E6 0%, #FFFFFF 100%);
    position: relative;
    margin-top: 500px;

    &__img {
        width: 100%;
        position: absolute;
        top: -50px;
    }
    &__title {
        font-weight: bold;
        font-size: 48px;
        line-height: 53px;
        text-align: center;
        color: #222222;
        margin-bottom: 30px;
    }
    &__text {
        font-size: 18px;
        line-height: 25px;
        text-align: center;
        color: #222222;
        margin-bottom: 50px;
    }
    &__items {
        display: flex;
        justify-content: space-between;
        gap: 60px;
        margin-bottom: 40px;

    }
    &__item {
        text-align: center;
        &-title {
            font-size: 22px;
            line-height: 29px;
            color: #222222;
            margin-bottom: 12px;
        }
        &-text {
            font-size: 16px;
            line-height: 22px;
            color: #555555;
        }
    }
    .features {
        font-size: 16px;
        line-height: 22px;
        text-transform: uppercase;
        color: #222222;
        display: flex;
        align-items: center;
        background: #FFF2CD;
        border-radius: 8px;
        padding: 16px 32px;
        border: none;
        outline: none;
        gap: 6px;
        margin: auto;
        margin-top: 100px;
        margin-bottom: 200px;

    }
}

@media only screen and (max-width: 750px) {
    .offer {
        margin-top: 0;
        &__img {
            top: -12px;
        }
        &__title {
            font-size: 28px;
            line-height: 34px;
        }
        &__text {
            font-size: 16px;
            line-height: 22px;
        }
        &__items {
            flex-direction: column;
        }
        .features {
            margin-top: 0;
            margin-bottom: 0;
        }
        
    }
}
</style>