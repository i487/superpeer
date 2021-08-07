<template>
    <div class="course">
        <div class="course-img-wrapper">
            <img :src="img" alt="" class="course__img">
            <div class="course__teacher">
                <img :src="teacher" alt="" class="course__teacher-img">
            </div>
        </div>
        <h3 class="course__name"> {{ name }} </h3>
        <p class="course__teacher-name"> {{ staff }} </p>
        <p class="course__description"> {{ description }} </p>
        <div class="course__enrollment">
            <div class="course__enrollment-manage">
                <p class="course__start">Starts</p>
                <time class="course__time"> {{ date }} </time>
            </div>
            <button class="course__enroll-btn">Enroll</button>
        </div>
    </div>
</template>

<script>
export default {
    name: "Courses",
    props: ["img", "teacher", "name", "staff", "description", "date"]
}
</script>

<style lang="scss">
.course {
    max-width: 402px;
    width: 100%;
    .course-img-wrapper {
        position: relative;
    }
    &__img {
        max-width: 400px;
        width: 100%;
        height: 225px;
    }
    &__teacher {
        background: white;
        border-radius: 50%;
        width: 86px;
        height: 86px;
        display: flex;
        justify-content: center;
        align-items: center;
        position: absolute;
        bottom: -45px;
        left: 50%;
        transform: translate(-50%);

        &-img {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            object-fit: cover;
        }
        &-name {
            font-size: 16px;
            line-height: 22px;
            text-align: center;
            color: #555555;
        }
    }
    &__name {
        font-weight: bold;
        font-size: 22px;
        line-height: 29px;
        color: #222222;
        margin-top: 48px;
        text-align: center;
        margin-bottom: 12px;
    }
    &__description {
        font-size: 16px;
        line-height: 22px;
        text-align: center;
        color: #555555;
        margin-bottom: 36px;
        margin-top: 16px;
    }
    &__enrollment {
        padding: 0 15px;
        display: flex;
        align-items: center;
        justify-content: space-between;
        &-manage {
            display: flex;
            gap: 10px;
            align-items: center;
        }

    }
    &__start {
        font-size: 16px;
        line-height: 22px;
        text-align: center;
        color: #98A3B6;
    }
    &__time {
        font-size: 16px;
        line-height: 22px;
        text-align: center;
        color: #000000;
    }
    &__enroll-btn {
        font-size: 16px;
        line-height: 22px;
        text-align: center;
        text-transform: uppercase;
        color: #222222;
        padding: 16px 32px;
        background: #FFEDC2;
        border-radius: 8px;
        outline: none;
        border: none;
        cursor: pointer;
    }
}
</style>