<template>
    <div class = "main__skills" id="skills">
        <h2>Skills</h2>
        <h3>I work in such programs as</h3>
        <div class = "skills">
            <ul class = "skills__list">
                <li class = "skills__list-item" v-for="(item, index) in listItems" :key=index>
                    <img :src=getImgSvg(item.pic) :alt=item.alt>
                    <h4>{{ item.title }}</h4>
                    <starsSkills></starsSkills>
                </li>
            </ul>
        </div>
    </div>
</template>>

<script>
import starsSkills from '../starsSkills.vue'
    export default {
        name: 'skillsMain',
        components: {starsSkills},
        data: function() {
            return {
             listItems: [
            {
                pic:'photoshop.svg', 
                alt:"Adobe Photoshop icon", 
                title:"Adobe Photoshop"
            },
            {
                pic:'illustrator.svg', 
                alt:"Adobe Illustrator icon", 
                title:"Adobe Illustrator"
            },
            {
                pic:'afftereffect.svg', 
                alt:"Adobe After Effects icon", 
                title:"Adobe After Effects"
            },
            {
                pic:'figma.svg', 
                alt:"Figma icon", 
                title:"Figma" 
            },
        ],   
            }
        },
        methods: {
        getImgSvg(svg) {
            return require('../../assets/images/' + svg)
        },
    },
    }
</script>

<style>
.main__skills h2 {
    font-family: "Roboto";
    font-weight: 700;
    font-size: 34px;
    text-align: center;
}

.main__skills h3 {
    font-family: "Roboto";
    font-weight: normal;
    font-size: 18px;
    text-align: center;
    margin: 0;
    margin-top: 16px;
    margin-bottom: 57px;
}

@media (min-width: 1200px) {
    .main__skills h3 {
        margin-top: 30px;
        margin-bottom: 75px;
    }
}

.main__skills h4 {
    font-family: "Roboto";
    font-weight: 700;
    font-size: 14px;
    text-align: center;
    color:#828282;
    margin-top: 23px;
    margin-bottom: 41px;
    width: 63%;
}

@media (min-width: 1200px) {
    .main__skills h4 {
        margin-bottom: 40px;
    }
}

.main__skills {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding-bottom: 32px;
    padding-top: 48px;
}

@media (min-width: 1200px) {
    .main__skills {
        padding-top: 55px;
        padding-bottom: 95px;
    }
}

.skills__list, .stars {
    padding-left: 0;
}

.skills__list-item, .stars__item {
    list-style-type: none;
}

@media (min-width: 1200px) {
    .skills{
        width: 100%;
    }
}

.skills__list {
    display: flex;
    flex-direction: row;
    align-items: center;
    flex-wrap: wrap;
    justify-content: center;
    row-gap: 81px;
    column-gap: 50px;
}

@media (min-width: 1200px) {
    .skills__list {
        width: 100%;
        flex-direction: row;
        justify-content: space-between;
    }
}

.skills__list-item {
    display: flex;
    flex-direction: column;
    align-items: center;
}

@media (min-width: 1200px) {
    .skills__list-item:last-child h4 {
        margin-bottom: 57px;
    }
}
</style>>