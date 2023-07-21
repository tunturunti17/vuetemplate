<template>
    <nav class="header__nav">
        <ul class="header__menu">
            <li v-for="item in menuItems" :key="item.id" :class=item.class>
                <a :href=item.href>{{ item.title }}</a>
            </li>
        </ul>
    </nav>
</template>

<script>
    export default {
        name: 'navBar',
        props: {

        },
        data: function() {
          return {
           menuItems: [
              {class: "header__nav-item active", href: '#', title: "Home"},
              {class: "header__nav-item", href: '#aboutme', title: "About me"},
              {class: "header__nav-item", href: '#skills', title: "Skills"},
              {class: "header__nav-item", href: '#portfolio', title: "Portfolio"},
              {class: "header__nav-item", href: '#contacts', title: "Contacts"},
           ],
          }
        }
      }
</script>

<style>
  .header__menu {
    display: none;
  }
  
@media (min-width: 768px) {
    .header__wrapper h1 {
        padding-top: 69px;
        padding-bottom: 0px;
    }

    .header__wrapper h2{
        margin:0px;
        padding-bottom:7px;
    }
    .header__wrapper{
        align-items: flex-start;
        flex-direction: column;
        margin-top: 2.5%;
        margin-bottom: 0;
    }

    .header__nav {
        width: 100%;
        display: flex;
        position: relative;
    }

    .header__menu:after {
        content: "";
        position: absolute;
        bottom: -30px;
        background-color:#828282;
        height: 1px;
        width:100%;
    }

   .header__menu {
        position: relative;
        display: flex;
        justify-content: space-between;
        width: 100%;
        font-family: "Roboto-Bold";
        font-weight: bold;
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
}
</style>>