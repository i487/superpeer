<template>
    <section class="series">
        <img src="../assets/series.png" alt="" class="series__top-img">
        <div class="container">
            <h2 class="series__title">See what magic our community is creating</h2>
            <p class="series__text">Explore these examples of Series, created by our Superpeers, and reserve your spot today</p>

            <div class="courses">
                <Courses v-for="(item, index) in course" :key="index" 
                :img = "item.courseImg" 
                :teacher = "item.teacherImg" 
                :name="item.courseName"
                :staff="item.teacherName"
                :description="item.description"
                :date="item.startDate"/>
            </div>
        </div>
    </section>
</template>

<script>
import Courses from './Courses.vue'
export default {
  components: { Courses },
    name: "Series",
    data () {
        return {
            course: [
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Dawn Dickson",
                    courseName: "Masterclass on Fundraising Strategies",
                    description: "Entry-level strategies from an expert in entrepreneurship, business development and fundraising. The first female founder to raise $1M> in an equity crowdfunding campaign will teach you the best in investment, crowdfunding and overall fundraising strategies to capitalize your business at every level.",
                    startDate: "September 9, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Thomas Hopkins",
                    courseName: "Paid Marketing",
                    description: "Over the past 7 years I've unlocked company growth potential for brands like Lyft and Masterclass – after this series, you will too. Discover what makes a successful paid marketing campaign and how to scale a revenue-generating system.",
                    startDate: "August 6, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Alice Johnson",
                    courseName: "Find Your True Love, your TwinFlame®",
                    description: "I'm an 8th-generation psychic, and together we'll discover how your aura operates and the magic you have within to facilitate self-love and romantic love. If you’re looking for your Twinflame®, your true love, or you’re ready to find yourself, this is the course for you.",
                    startDate: "July 26, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Mark Wahlbeck",
                    courseName: "Fiction Writing For Absolute Beginners: How To Publish Your First Story",
                    description: "Writing can be hard! Publishing can be even harder! In this Series not only will you learn how to write good fiction, you’ll also learn how to publish your writing.",
                    startDate: "August 2, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Jason Akel",
                    courseName: "Self-Hypnosis and HypnoTherapy Adventures",
                    description: "Stop being so critical of yourself and overanalyzing everything. Discover the power of hypnosis and hypnotherapy: you could be living a more confident, free-thinking life. For first-timers and experienced meditators – relax, learn and get motivated.",
                    startDate: "July 24, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Tristan Pollock",
                    courseName: "Movement Building",
                    description: "Calling all startup founders, entrepreneurs, execs, and business leaders. Learn to build communities, make a pitch deck and create a movement around a company mission. Global impact-driven movements have all started somewhere, and today it's here",
                    startDate: "July 28, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Jose Caya",
                    courseName: "Pitch Deck Examples & How to Class",
                    description: "Entry-level strategies from an expert in entrepreneurship, business development and fundraising. The first female founder to raise $1M> in an equity crowdfunding campaign will teach you the best in investment, crowdfunding and overall fundraising strategies to capitalize your business at every level.",
                    startDate: "September 9, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Devrim Yasar",
                    courseName: "Starting your Business",
                    description: "Entry-level strategies from an expert in entrepreneurship, business development and fundraising. The first female founder to raise $1M> in an equity crowdfunding campaign will teach you the best in investment, crowdfunding and overall fundraising strategies to capitalize your business at every level.",
                    startDate: "September 9, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Jose Caya",
                    courseName: "Public Speaking",
                    description: "Entry-level strategies from an expert in entrepreneurship, business development and fundraising. The first female founder to raise $1M> in an equity crowdfunding campaign will teach you the best in investment, crowdfunding and overall fundraising strategies to capitalize your business at every level.",
                    startDate: "September 9, 2021"
                },
                {
                    courseImg: "https://picsum.photos/450/250",
                    teacherImg: "https://picsum.photos/100/100",
                    teacherName: "Jasmine Lawrence",
                    courseName: "You can’t Entrepreneur without PM",
                    description: "Entry-level strategies from an expert in entrepreneurship, business development and fundraising. The first female founder to raise $1M> in an equity crowdfunding campaign will teach you the best in investment, crowdfunding and overall fundraising strategies to capitalize your business at every level.",
                    startDate: "September 9, 2021"
                },
            ]
        }
    }
}
</script>

<style lang="scss">
.series {
    position: relative;
    padding-top: 100px;
    padding-bottom: 100px;
    // margin-top: 50px;

    &__top-img {
        position: absolute;
        width: 100%;
        z-index: -1;
        top: -160px;
    }
    &__title {
        font-weight: bold;
        font-size: 48px;
        line-height: 53px;
        text-align: center;
        color: #222222;
        margin-bottom: 14px;
        padding: 0 200px;
    }
    &__text {
        font-size: 18px;
        line-height: 25px;
        text-align: center;
        color: #222222;
        padding: 0 200px;
        margin-bottom: 58px;
    }
    .courses {
        display: grid;
        grid-template-columns: 1fr 1fr;
        justify-content: space-between;
        grid-gap: 100px;
    }
}

@media only screen and (max-width: 750px) {
    .series {
        &__top-img {
            top: -40px;
        }
        &__title {
            font-size: 28px;
            line-height: 38px;
            padding: 0;
        }
        &__text {
            font-size: 16px;
            line-height: 22px;
            padding: 0;
        }
        .courses {
            grid-template-columns: 1fr;
            grid-gap: 30px;
            .course {
                &__name {
                    font-size: 18px;
                    line-height: 22px;
                }
                &__time {
                    font-size: 14px;
                    line-height: 18px;
                }
                &__enroll-btn {
                    font-size: 12px;
                    line-height: 14px;
                    padding: 12px 24px;
                }
            }
        }
    }
}
</style>