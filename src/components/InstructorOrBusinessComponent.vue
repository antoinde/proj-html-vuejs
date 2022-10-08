<template>
    <section>
        <div class="default-container">

            <div class="left">
                <div class="img-container">
                    <img src="@/assets/img/image_box_1-221x231.png" alt="">
                </div>
                <div class="text-container">
                    <h2>Become an Instructor</h2>
                    <p>Teach what you love. Masterstudy gives you the tools to create a course.</p>
                    <a class="typeButtonRose" href="#">START TEACHING</a>
                </div>
            </div>


            <div class="right">
                <div class="img-container">
                    <img src="@/assets/img/image_box_2-234x231.png" alt="">
                </div>
                <div class="text-container">
                    <h2>Access For Business</h2>
                    <p>Get unlimited access to 2,500 of top courses for your team.</p>
                    <a class="typeButtonRose" href="#">DOING BUSINESS</a>
                </div>
            </div>



        </div>
    </section>
</template>

<script>
export default {
    name: "InstructorOrBusinessComponent",

}

</script>

<style lang="scss" scoped>
.default-container {
    display: flex;
    column-gap: 20px;
    margin-bottom: 60px;

    .left,
    .right {
        padding: 30px;
        border: 1px solid grey;
        width: 50%;
        display: flex;

        .text-container{
            p{
                margin-bottom: 40px;
                color: grey;
            }
        }
    }
    .img-container {
        width: 33%;
        margin-right: 30px;
    }
}
</style>