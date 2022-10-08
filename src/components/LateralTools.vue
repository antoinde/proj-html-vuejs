<template>

    <div class="LateralTools">

        <div class="Tools_content">
            <i class="fa-solid fa-desktop"></i>
            <i class="fa-solid fa-life-ring"></i>
            <i class="fa-solid fa-wrench"></i>
            <i class="fa-solid fa-cart-shopping"></i>
            <i class="fa-solid fa-mobile-screen-button"></i>
        </div>

    </div>

</template>

<script>
export default {
    name: 'LateralTools'
}
</script>

<style lang="scss" scoped>
.LateralTools {
    position: fixed;
    right: 0;
    bottom: 30%;
}

.Tools_content {
    display: flex;
    flex-direction: column;
    font-size: 1.5rem;
    padding: 15px;
    row-gap: 30px;
    background-color: #fff;

    box-shadow: -3px 5px 22px -1px rgba(0, 0, 0, 0.75);
    -webkit-box-shadow: -3px 5px 22px -1px rgba(0, 0, 0, 0.75);
    -moz-box-shadow: -3px 5px 22px -1px rgba(0, 0, 0, 0.75);

    i {
        margin-left: 10px;
    }
    i:hover{
       color: grey;

    }
}
</style>