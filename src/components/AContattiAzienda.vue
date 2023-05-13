<script>
export default {
    name: "AContattiAzienda"
}

</script>

<template>
    <div class="cont">
        <div class="contatti d-flex justify-content-between">
            <div class="orario">
                <i class="fa-solid fa-clock"></i>
                <span>Open Hours Mon - Sat - 9.00 - 18.00</span>
            </div>
            <div class="recapiti">
                <span><i class="fa-solid fa-phone"></i> +1(305) 1234-5678</span>
                <span><i class="fa-regular fa-envelope"></i> hello@example.com</span>
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-linkedin-in"></i>
            </div>
        </div>

    </div>
</template>

<style lang="scss" scoped>
.cont {
    background-color: #21333E;

    .contatti {
        width: 75%;
        margin: 0 auto;
        padding: 10px 0;
    }

    i,
    span {
        color: whitesmoke;
        padding: 0 8px;
        font-size: 14px;
    }
}
</style>