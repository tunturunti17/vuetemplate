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
    font-family: "Roboto-Bold";
    font-weight: bold;
    font-size: 34px;
    text-align: center;
    margin:0px;
}

@media (min-width: 1200px) {
    .footer {
        margin-top:5%;
    }
    .footer h2 {
        padding-top:1%;
    }

}

.footer__text {
    font-family: "Roboto-Medium";
    font-weight: normal;
    font-size: 18px;
    text-align: center;
}

.footer__text {
    margin: 0;
    margin-bottom: 14%;
    padding: 0 5%;
}

@media (min-width: 768px) {
    .footer__text {
        margin-bottom: 3%;
        padding: 0;
    }
}
</style>