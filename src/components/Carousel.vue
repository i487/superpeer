<template>
    <section class="carousel">
        <div class="container carousel__container">
            <h2 class="carousel__title">Don’t just take our word for it</h2>
            <span class=" carousel__left-arrow ">
                <img src="../assets/left.png" alt="">
            </span>
            <span class="carousel__right-arrow">
                <img src="../assets/righ.png" alt="">
            </span>
            <VueSlickCarousel :arrows="true" class="carousel__slider">
                <div class="carousel__text">“I've been using Superpeer with about 10-12 calls per week, and so far the
                    experience has been flawless.”</div>
                <div class="carousel__text">“I've been using Superpeer with about 10-12 calls per week, and so far the
                    experience has been flawless.”</div>
                <div class="carousel__text">“I've been using Superpeer with about 10-12 calls per week, and so far the
                    experience has been flawless.”</div>
                <div class="carousel__text">“I've been using Superpeer with about 10-12 calls per week, and so far the
                    experience has been flawless.”</div>
            </VueSlickCarousel>

            <div class="blog">
                <img src="../assets/blog.png" alt="" class="blog__img">
                <h5 class="blog__owner">Janine Sickmeyer</h5>
                <p class="blog__job">Tech entrepreneur & Angel investor</p>
            </div>
        </div>
    </section>
</template>

<script>
    import VueSlickCarousel from 'vue-slick-carousel'
    import 'vue-slick-carousel/dist/vue-slick-carousel.css'
    import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'

    export default {
        name: 'Carousel',
        components: {
            VueSlickCarousel
        },
    }
</script>

<style lang="scss">
    .carousel {
        background: linear-gradient(180deg, #FFFAEC 0%, rgba(255, 255, 255, 0) 100%);
        text-align: center;
        padding: 60px 0;
        width: 95%;
        margin: auto;

        &__container {
            text-align: center;
            position: relative;
        }

        &__title {
            font-size: 48px;
            line-height: 53px;
            text-align: center;
            letter-spacing: 1px;
            color: #222222;
            margin-bottom: 100px;
        }

        &__text {
            font-size: 32px;
            line-height: 40px;
            text-align: center;
            color: #222222;
            padding: 0 50px 60px;
        }

        &__left-arrow {
            position: absolute;
            left: -60px;
            cursor: pointer;
        }
        &__right-arrow {
            position: absolute;
            right: -60px;
            cursor: pointer;
        }
        &__slider {
            margin-bottom: 50px;
        }
        .blog {
            
            text-align: center;
            display: flex;
            flex-direction: column;
            gap: 16px;
            &__img {
                width: 58px;
                height: 58px;
                margin: auto;
            }


        }
    }

    @media only screen and (max-width: 750px) {
        .carousel {
            &__title {
                font-size: 28px;
                line-height: 34px;
            }
            &__text {
                font-size: 16px;
                line-height: 24px;
            }
            &__right-arrow {
                display: none;
            }
            &__left-arrow {
                display: none;
            }
        }
    }
</style>