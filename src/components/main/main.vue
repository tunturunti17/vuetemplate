<template>
    <main class="main">
      <section class="main main--about">
          <div class = "container">
              <aboutMain></aboutMain>
          </div>
      </section>
      <section class = "main main--skills">
        <div class = "container">
          <skillsMain></skillsMain>
        </div>
      </section>
      <section class = "main main--portfolio">
          <div class = "container">
              <portfolioMain></portfolioMain>
          </div>
      </section>
    </main>
</template>>

<script>
import aboutMain from './aboutme.vue'
import portfolioMain from './portfolio.vue'
import skillsMain from './skills.vue'

export default {
    name:'mainSite',
    components: {
        aboutMain,
        portfolioMain,
        skillsMain,
    },
}
</script>

<style>
body {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    min-height: 100vh;
    margin:0%;
  }

  .header__image img{
    width: 100%;
    height: auto;
  }

.container {
    max-width:375px;
    min-width: 320px;
    padding: 0 30px;
    box-sizing: border-box;
    margin: 0 auto;
  }

  @media (min-width: 480px){
    .container {
      max-width: 100%;
    }
  }
  @media (min-width:768px) {
    .container {
      max-width:700px;
      padding: 0px;
      box-sizing: border-box;
      margin: 0 auto;
    }
  }


  @media (min-width:1200px) {
    .container {
      max-width:940px;
      padding: 0px;
      box-sizing: border-box;
      margin: 0 auto;
    }
  }

  .main--about,
  .main--portfolio {
    max-width: 100%;
    background-color: #F6F6F6;
  }

</style>