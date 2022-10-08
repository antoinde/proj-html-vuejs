<template>
    <section>
        <div class="text-area">
            <h1>Investing for Your Future</h1>
            <p>It is no exaggeration to say this MasterStudy experience was transformative-both professionally and
                personally. This workshop will long remain a high point of my life. Thanks again.... I am feeling
                energized and eager to start teaching my class next week. I can't wait to use all of my new teaching
                tools. I will absolutely recommend this workshop to other educators!</p>
            <h5>Linda Green</h5>
            <div>Product Manager, Apple Inc</div>
        </div>
    </section>
</template>

<script>


export default {
    name: "TestimonialComponent",
}
</script>

<style lang="scss" scoped>
section {
    position: relative;
    padding: 50px 0px;
    height: 500px;
    background-image: url('@/assets/img/testimonial-1-1917x640-1-1914x639.jpg');
}

.text-area {
    position: absolute;
    background-color: #fff;
    padding: 60px;
    width: 500px;
    left: 25%;
    top: 70px;

    h1 {
        font-size: 2.6rem;
        margin-bottom: 10px;
    }
    h5{
        margin-bottom: 5px;
    }
    p {
        margin-bottom: 55px;
        line-height: 1.7rem;
    }
}
</style>