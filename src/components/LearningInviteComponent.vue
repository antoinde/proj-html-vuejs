<template>
    <section>
       <div class="text-area">
        <h1>Limitless leaning,<br>more possibilities</h1>
        <p>Online courses open the opportunity for learning to almost anyone, regardless of their scheduling commitmens.</p>
        <a class="typeButtonRose" href="#">READ MORE</a>
       </div>
    </section>
</template>

<script>


export default {
    name: "LearningInviteComponent",
}
</script>

<style lang="scss" scoped>
section{
    position: relative;
    padding: 50px 0px;
    height: 350px;
    background-image: url('@/assets/img/bg.png');
}
.text-area{
    position: absolute;
    width: 500px;
    left: 25%;
    top: 70px;
    h1{
        font-size: 2.6rem;
        margin-bottom: 10px;
    }
    p{
        margin-bottom: 55px;
    }
}

</style>