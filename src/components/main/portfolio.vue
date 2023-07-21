<template>
    <div class="main__portfolio" id="portfolio">
            <h2>Portfolio</h2>
        <div class = "portfolio">
            <ul class = "portfolio__list">
                <li v-for="(item, index) in imgItems" :key="index" :class=item.class>
                    <img :src= getImgUrl(item.pic)
                    :alt=item.alt>
                    <h3>{{ item.title }}</h3>
                </li>
            </ul>
        </div>
    </div>
</template>>

<script>
export default {
    name: 'portfolioMain',
    props: {

    },
    data: function() {
        return {
        imgItems: [
            {
                class:"portfolio__list-item",
                pic:'store-1200w.png', 
                alt:"Online fashion store - Homepage", 
                title:"Online fashion store - Homepage" 
            },
            {
                class:"portfolio__list-item", 
                pic:'reebok-1200w.png', 
                alt:"Reebok Store - Concept", 
                title:"Reebok Store - Concept" 
            },
            {
                class:"portfolio__list-item", 
                pic:'braun-1200w.png', 
                alt:"Braun Landing Page - Concept", 
                title:"Braun Landing Page - Concept" 
            },
        ],
        }
    },
    methods: {
        getImgUrl(pic) {
            return require('../../assets/images/' + pic)
        },
    },
}
</script>
<style>
.container--portfolio {
    background-color:#F6F6F6;
}

.main__portfolio h2 {
    font-family: "Roboto-Bold";
    font-weight: bold;
    font-size: 34px;
    text-align: center;
    margin:0;
}

.main__portfolio h3 {
    font-family: "Roboto-Medium";
    font-weight: normal;
    font-size: 18px;
    text-align: center;
    text-decoration: underline;
    margin-top: 27px;
    margin-bottom:0;
}
@media (min-width: 500px){
    .main__portfolio h3 {
        margin-top: 41px;
    }
}
.main__portfolio {
    display: flex;
    flex-direction: column;
    row-gap: 58px;
    padding: 33% 0;
}

@media (min-width: 500px){
    .main__portfolio{
        row-gap: 47px;
        padding-top:6%;
        padding-bottom:9%
    }
}

@media (min-width: 500px){
    .main__portfolio{
        padding-top:11%;
    }
}

.portfolio__list {
    padding-left: 0;
    display: flex;
    row-gap: 78px;
    flex-direction: column;
}
@media (min-width: 500px){
    .portfolio__list{
        row-gap: 102px;
    }
}
.portfolio__list-item {
    list-style-type: none;
}

.portfolio__list-item img{
    width:100%;
}

@media (min-width: 500px) {
    .portfolio__list-item {
        display: flex;
        flex-direction: column;
        align-items: center;
    }
    .portfolio__list-item img {
        width: 100%;
    }
}
</style>