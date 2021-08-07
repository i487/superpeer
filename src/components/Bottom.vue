<template>
    <section class="bottom">
        <img src="../assets/bottom.png" alt="" class="bottom__img-abs">
        <div class="container bottom__container">
            <img src="../assets/hand.png" alt="" class="bottom__img">
            <h2 class="bottom__title">Become a Superpeer</h2>
            <button class="bottom__btn">Create an account</button>
        </div>

    </section>
</template>

<script>
export default {
    name: "Bottom"
}
</script>

<style lang="scss">
.bottom {
    position: relative;
    margin-top: 60px;
    padding: 100px 0;

    &__img-abs {
        position: absolute;
        z-index: -1;
        left: 3%;
        width: 100%;
        animation-name: beater;
        animation-duration: 2s;
        animation-iteration-count: infinite;
    }
    &__container {
        text-align: center;
    }
    &__img {
        margin-bottom: 40px;
        max-width: 150px;
        width: 100%;
    }
    &__title {
        font-weight: bold;
        font-size: 56px;
        line-height: 62px;
        color: #222222;
        margin-bottom: 60px;
    }
    &__btn {
        font-weight: bold;
        font-size: 16px;
        line-height: 22px;
        color: #222222;
        padding: 16px 32px;
        background: #FFD338;
        border-radius: 8px;
        border: none;
        outline: none;
        cursor: pointer;
    }

}
@keyframes beater {
    0% {
        transform: scale(1.02);
    }
    50% {
        transform: scale(1.06);
    }
}

@media only screen and (max-width: 750px){
    .bottom {
        overflow: hidden;
        padding: 0;
        margin-top: 20px;
        &__img {
            width: 50px;
            margin-bottom: 0;
        }
        &__title {
            font-size: 28px;
            line-height: 34px;
            margin-bottom: 10px;
        }
        &__btn {
            font-size: 12px;
            line-height: 14px;
            padding: 14px 28px;
        }
    }
}
</style>