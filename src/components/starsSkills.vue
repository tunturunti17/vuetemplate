<template>
    <ul class="stars">
        <li class = "stars__item">
        <svg class = "star">
            <use xlink:href="@/assets/images/sprite.svg#star"></use>
        </svg>
        </li>
        <li class = "stars__item">
        <svg class = "star">
            <use xlink:href="@/assets/images/sprite.svg#star"></use>
        </svg>
        </li>
        <li class = "stars__item">
        <svg class = "star">
            <use xlink:href="@/assets/images/sprite.svg#star"></use>
        </svg>
        </li>
        <li class = "stars__item">
        <svg class = "star">
            <use xlink:href="@/assets/images/sprite.svg#star"></use>
        </svg>
        </li>
        <li class = "stars__item">
        <svg class = "star none-active">
            <use xlink:href="@/assets/images/sprite.svg#star"></use>
        </svg>
        </li>
    </ul>
</template>
<script>
export default ({
    name: 'starsSkills'
})
</script>

<style>
.star {
  fill:#000;
  width: 21px;
  height: 21px;
}

.none-active {
  fill:#E5E5E5;
}

.stars {
    display: flex;
    flex-direction: row;
    column-gap: 15px;
}
</style>>