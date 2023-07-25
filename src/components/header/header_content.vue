<template>
    <div class = "header__content">
        <h1>Denis<br>Novik</h1>
        <h2>UX | UI designer<br>
          24 years old, Minsk</h2>
        <nav class="language">
            <ul class="language__menu">
                <li v-for="item in menuLangItems" :key="item.id" :class=item.class>
                    <a :href=item.href>{{ item.title }}</a>
                </li>
            </ul>
        </nav>
      </div>
</template>

<script>
export default {
  name: 'headerContent',
  props: {
 
  },
  data: function() {
    return {
     menuLangItems: [
        {class:"language__menu-item", href:'#', title:"RU" },
        {class:"language__menu-item active", href:'#', title:"|"},
        {class:"language__menu-item active", href:'#', title:"ENG"},
    ],
    }
  }
}
</script>
<style>

  .header__wrapper h1 {
    font-family: "Roboto";
    font-weight: 700;
    font-size: 47px;
    box-sizing: content-box;
    margin: 0;
    padding-top: 25px;
    padding-bottom: 26px;
  }

  .header__wrapper h2 {
    font-family: "Roboto";
    font-weight: normal;
    font-size: 18px;
    margin-top: 0;
    margin-bottom: 38px;
  }

  .language {
    display: none;
  }

     @media (min-width: 768px) {
    .header__wrapper h1 {
        padding-top: 69px;
        padding-bottom: 0px;
    }

    .header__wrapper h2 {
        margin:0px;
        padding-bottom:7px;
    }

    .header__wrapper {
        align-items: flex-start;
        flex-direction: column;
        margin-top: 25px;
        margin-bottom: 0;
    }

    .header__nav {
        width: 100%;
        display: flex;
    }

    .header__menu {
        position: relative;
        display: flex;
        justify-content: space-between;
        width: 100%;
        font-family: "Roboto";
        font-weight: 700;
        font-size: 18px;
        padding-left: 0;
        margin: 0;
    }

    .header__nav-item {
        list-style-type: none;
        text-align: center;
    }

    .header__nav-item a {
        text-decoration: none;
        color:#828282;
    }

    .header__content {
        width: 100%;
        display: flex;
        align-items: flex-end;
        justify-content: space-between;
        margin-bottom: 45px;
    }

    .language {
        display: flex;
        transform: rotate(270deg);
        padding-left: 2px;
        padding-top: 56px;
    }

    .language__menu {
        display: flex;
        flex-direction: row;
        column-gap: 5px;        
        padding-left: 0px;
        margin: 0;
    }

    .language__menu-item {
        list-style-type: none;
        color:#000
    }

    .language__menu-item a {
        text-decoration: none;
        color:#828282;
        font-family: "Roboto";
        font-weight: normal;
        font-size: 18px;
    }

    .active {
        font-family: "Roboto";
        font-weight: normal;
        font-size: 18px;
        color:#000;
    }
   .active a {
        font-family: "Roboto";
        font-weight: normal;
        font-size: 18px;
        color:#000;
    }
    .mobile {
        display: none;
    }
  }
</style>