<template>
    <footer class="footer">
        <div class="container">
            <div class="footer__wrapper">
                <footerContent></footerContent>
                <socialFooter></socialFooter>
            </div>
        </div>
    </footer>
</template>>

<script>
import footerContent from './footerContent.vue'
import socialFooter from './socialFooter.vue'

export default {
    name:'footerSite',
    components: {
        footerContent,
        socialFooter
    },
}
</script>

<style>
    .footer__wrapper {
        display: flex;
        flex-direction: column;
        align-items: center;
        row-gap: 32px;
        margin-top: 50px;
    }


    @media (min-width: 500px) {
        .footer__wrapper {
            margin-top: 60px;
        }
    }
</style>