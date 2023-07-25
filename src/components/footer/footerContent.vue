<template>
    <h2>Contacts</h2>
    <div class = "footer__content">
        <p class = "footer__text">
        Want to know more or just chat?<br> You are welcome!
        </p>
        <btnFooter></btnFooter>
    </div> 
</template>>

<script>
import btnFooter from '../btn.vue'

export default {
    name:'footerContent',
    components: {
        btnFooter
    },
}
</script>


<style>
.footer h2 {
    font-family: "Roboto";
    font-weight: 700;
    font-size: 34px;
    text-align: center;
    margin:0px;
}

@media (min-width: 1200px) {
    .footer {
        margin-top:70px;
    }
    .footer h2 {
        padding-top: 10px;
    }

}

.footer__text {
    font-family: "Roboto";
    font-weight: normal;
    font-size: 18px;
    text-align: center;
}

.footer__text {
    margin: 0;
    margin-bottom: 40px;
    padding: 0 15px;
}

@media (min-width: 768px) {
    .footer__text {
        margin-bottom: 8px;
        padding: 0;
    }
}
</style>