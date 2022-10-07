<template>
    <section>
        <div class="default-container">

            <div class="left"></div>


            <div class="right"></div>



        </div>
    </section>
</template>

<script>
export default {
    name: "InstructorOrBusinessComponent",
    
}

</script>

<style lang="scss" scoped>
.default-container{
    display: flex;

    .left,.right{
        padding: 10px;
        border: 1px solid grey;
    }
}

</style>