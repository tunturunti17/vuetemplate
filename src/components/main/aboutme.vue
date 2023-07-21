<template>
    <div class = "main__about" id="aboutme">
        <h2>About me</h2>
            <ul class = about>
                <li class = "about__item"><p>
                    Hi, I'm Denis – UX/UI designer from Minsk.
                    I'm interested in design and everything connected with it.
                </p></li>
                <li class = "about__item"><p>
                    I'm studying at courses
                    "Web and mobile design interfaces"
                    in IT-Academy.
                </p></li>
                <li class = "about__item"><p>
                    Ready to implement excellent projects
                    with wonderful people.
                </p></li>
            </ul>
    </div>
</template>>

<script>
    export default {
        name: 'aboutMain',
    }
</script>
>
<style>
.container--about {
    background:#F6F6F6;
}

.main__about {
    padding:15% 0;
}

@media (min-width: 1200px){
    .main__about {
        padding-top:12%;
        padding-bottom:7%;
    }
}

.main__about h2 {
    font-family: "Roboto-Bold";
    font-weight: bold;
    font-size: 34px;
    text-align: center;
}

@media (min-width: 1200px) {
    .main__about h2{
        margin:0;
    }
}

.about {
    padding: 0;
    margin: 0;
    margin-top: 37px;
}

@media (min-width: 1200px){
    .about{
       margin-top: 25px; 
    }
}

.about__item {
    font-family: "Roboto-Medium";
    font-weight: normal;
    font-size: 18px;
}

.about__item {
    list-style-type: none;
    text-align: center;
    margin-bottom: 47px;
}

@media (min-width: 1200px){
    .about__item {
        padding: 0 26%;
    }
    .about__item:last-child {
        padding: 0 32%;
    }
}

.about__item p{
    margin-top: 0;
    margin-bottom: 10%;
}
</style>>