<template>
    <section>
        <div class="default-container">

            <div class="center-text">
                <h4>Recent Courses</h4>
                <nav>
                    <span>All Categories</span>
                    <span>Business</span>
                    <span>Design</span>
                    <span>Development</span>
                    <span>IT & Software</span>
                    <span>Lifestyle</span>
                    <span>Marketing</span>
                    <span>Office Productivity</span>
                </nav>
            </div>

            <RecentCoursesCardComponent />

            <div class="button">
                <a class="typeButtonRose" href="#">SHOW ALL</a>
            </div>
        </div>

        <div class="newsletter">
            <div class="container">
                <div class="left">
                    <h4>Subscribe our newsletter</h4>
                    <p>There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injected humour, or randomised words</p>
                </div>
                <div class="right">
                    <h4>YOUR E-MAIL ADDRESS</h4>
                    <div class="searchBar">
                    <input type="text" placeholder="Enter your E-mail">
                    <button style="color: #fff;">SUBSCRIBE</button>
                </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import RecentCoursesCardComponent from "./RecentCoursesCardComponent.vue";


export default {
    name: "RecentCoursesComponent",
    components: { RecentCoursesCardComponent }
}
</script>

<style lang="scss" scoped>
section {
    padding-top: 50px;

    .center-text {
        text-align: center;
        margin-bottom: 40px;

        h4 {
            font-size: 2.2rem;
        }

        nav {
            color: grey;

            span {
                margin: 0 10px;
                border-radius: 25px;
                padding: 10px;
            }

            span:hover {
                background-color: rgb(213, 213, 213);
                cursor: pointer;
            }
        }
    }

    .button {
        text-align: center;
        margin: 60px 0;
    }

    .newsletter {
        padding: 20px 0;
        background-color: var(--coralRed-color);
        color: #fff;

        .container {
            margin: 0 auto;
            width: 900px;
            display: flex;

            .left {
                width: 60%;
                line-height: 1.4em;
            }

            .right {
                width: 40%;
            }
        }
    }
}
</style>