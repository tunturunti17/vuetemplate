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
</template>

<script>
    export default {
        name: 'aboutMain',
    }
</script>

<style>
.container--about {
    background:#F6F6F6;
}

.main__about {
    padding: 48px 0;
}

@media (min-width: 1200px) {
    .main__about {
        padding-top: 112px;
        padding-bottom: 65px;
    }
}

.main__about h2 {
    font-family: "Roboto";
    font-weight: 700;
    font-size: 34px;
    text-align: center;
}

@media (min-width: 1200px) {
    .main__about h2{
        margin: 0;
    }
}

.about {
    padding: 0;
    margin: 0;
    margin-top: 37px;
}

@media (min-width: 1200px) {
    .about {
       margin-top: 25px; 
    }
}

.about__item {
    font-family: "Roboto";
    font-weight: normal;
    font-size: 18px;
}

.about__item {
    list-style-type: none;
    text-align: center;
    margin-bottom: 47px;
}

@media (min-width: 1200px) {
    .about__item {
        padding: 0 245px;
    }
    
    .about__item:last-child {
        padding: 0 300px;
    }
}

.about__item p {
    margin-top: 0;
    margin-bottom: 45px;
}
</style>