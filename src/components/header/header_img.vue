<template>
    <div class = "header__image">
        <picture>
            <source media="(min-width: 500px)" srcset="~@/assets/images/man-1200w.png">
            <img src="~@/assets/images/man-320w.png"
            alt="Denis Novik photo">
        </picture>
    </div>
</template>>

<script>


export default {
    name: "headerImg"
}
</script>
>

<style>
  .header__image {
    display: inline-block;
  }
 @media (min-width: 768px){
    .header__image {
        width: 100%;
    }
    .header__image img{
        width: 100%;
    }

 }
</style>>