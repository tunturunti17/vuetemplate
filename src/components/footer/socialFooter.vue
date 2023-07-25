<template>
    <nav class="social">
        <ul class="social__menu">
            <li class="social__nav-item">
            <a href="#">
                <svg class = "social__icon">
                <use xlink:href= "@/assets/images/sprite.svg#linkedin"></use>
                </svg>
            </a>
            </li>
            <li class="social__nav-item">
            <a href="#">
                <svg class = "social__icon">
                <use xlink:href="@/assets/images/sprite.svg#instagram"></use>
                </svg>
            </a>
            </li>
            <li class="social__nav-item">
            <a href="#">
                <svg class = "social__icon">
                <use xlink:href="@/assets/images/sprite.svg#behance"></use>
                </svg>
            </a>
            </li>
            <li class="social__nav-item">
            <a href="#">
                <svg class = "social__icon">
                <use xlink:href="@/assets/images/sprite.svg#dribble"></use>
                </svg>
            </a>
            </li>
        </ul>
    </nav>
        <div class = "footer__share">Like me on<br>LinkedIn, Instagram, Behance, Dribble</div>
</template>>

<script>
export default {
  name: 'socialFooter',
//   methods: {
//         getIconUrl(href) {
//             return require('@/assets/images/' + href)
//         },
//     },
//     data: function () {
//         return {
//             iconItems: [
//                 {href:'sprite.svg#linkedin'},
//                 {href:'sprite.svg#instagram'},
//                 {href:'sprite.svg#behance'},
//                 {href:'sprite.svg#dribble'},
//             ]
//         }
//     }
}
</script>

<style>
.social{
    margin-top: 6px;
}

@media (min-width: 500px) {
    .social {
        margin-top: 40px;
    }
}

.social__menu {
    padding-left: 0;
    display: flex;
    column-gap: 51px;
    margin: 0;
    justify-content: center;
}

@media (min-width: 500px) {
    .social__menu {
        column-gap: 60px;
    }
}

.social__nav-item {
    list-style-type: none;
    text-align: center;
}

.footer__share {
    font-family: "Roboto";
    font-weight: normal;
    font-size: 17px;
    text-align: center;
    color: #828282;
    display: block;
    margin-bottom: 90px;
}

@media (min-width: 768px) {
    .footer__share {
        font-size: 14px;
    }
}

.social__icon {
    width: 40px;
    height: 40px;
}
</style>