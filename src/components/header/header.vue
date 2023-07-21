<template>
    <header class="header">
        <popupSite/>
        <div class = "container">
            <div class= "header__wrapper">
                <navBar/>
                <popupBtn/>
                <headerContent/>
                <headerImg/>
            </div>
        </div>
    </header>
</template>

<script>
import popupSite from './popup.vue'
import navBar from '../navigation.vue'
import popupBtn from '../btn__popup.vue'
import headerContent from './header_content.vue'
import headerImg from './header_img.vue'

export default {
    name:'headerSite',
    components: {
        popupSite, 
        navBar, 
        popupBtn, 
        headerContent, 
        headerImg
    },
}
</script>
<style>

.header__wrapper {
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    align-items: flex-start;
    column-gap: 25px;
    margin-bottom: 11%;
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
</style>>