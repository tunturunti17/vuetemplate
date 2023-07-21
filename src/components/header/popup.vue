<template>
    <div id="popup" class="popup">
        <div class="popup__body">
          <nav class="popup__nav">
            <ul class="popup__menu">
                <li v-for="(item, index) in menuItems" :key="index" :class=item.class><a :href=item.href>{{ item.title }}</a></li>
            </ul>
            <a href="" class="popup__close close-popup">
              <svg class = "close">
                <use xlink:href="../icon/sprite.svg#close"></use>
              </svg>
            </a>
          </nav>
          <nav class="popup-language">
            <ul class="popup-language__menu">
              <li v-for="item in menuLangItems" :key="item.id" :class=item.class><a :href=item.href>{{ item.title }}</a></li>
            </ul>
        </nav>
        </div>
      </div>
</template>

<script>
export default {
  name: 'popupSite',
  props: {
    msg: String
  },
  data: function() {
    return {
     menuItems: [
        {class: "popup__nav-item active", href: '#', title: "Home"},
        {class: "popup__nav-item", href: '#aboutme', title: "About me"},
        {class: "popup__nav-item", href: '#skills', title: "Skills"},
        {class: "popup__nav-item", href: '#portfolio', title: "Portfolio"},
        {class: "popup__nav-item", href: '#contacts', title: "Contacts"},
     ],
     menuLangItems: [
        {class:"popup-language__menu-item", href:'#', title:"RU" },
        {class:"popup-language__menu-item active", href:'#', title:"|"},
        {class:"popup-language__menu-item active", href:'#', title:"ENG"},
    ],
    }
  }
}
</script>
<style>
.popup {
    width: 100%;
    height: 100%;
}

.popup__body {
    padding: 0 7%;
    margin: 10% 0;
    display: flex;
    flex-direction: column;
    row-gap: 150px;
}

.popup__menu {
    padding-left: 0;
    margin:0px;
    display: flex;
    flex-direction: column;
    row-gap: 68px;
}

.popup__nav {
    position: relative;
}
.popup__nav-item {
    list-style-type: none;
    text-align: left;
}

.popup__nav-item a {
    font-family: "Roboto-Bold";
    font-weight: bold;
    font-size: 34px;
    text-decoration: none;
    color:#828282;
}

.popup__close {
    display: block;
    height: 28px;
    width: 28px;
    margin: 0;
    position: absolute;
    top: 7px;
    left: 90%
}

.close{
    height: 28px;
    width: 28px; 
}

.popup-language__menu {
    padding-left: 0;
    margin:0px;
    display: flex;
    flex-direction: column;
    row-gap: 7px;
}

.popup-language__menu-item {
    list-style-type: none;
    text-align: left;
}

.popup-language__menu-item a {
    font-family: "Roboto-Bold";
    font-weight: bold;
    font-size: 34px;
    text-decoration: none;
    color:#828282;
    writing-mode: vertical-rl;
}

.popup-language__menu-item {
    writing-mode: vertical-rl;
    font-family: "Roboto-Bold";
    font-weight: bold;
    font-size: 34px;
    color:#000;
}

.active a {
    color:#000;
}

@media (min-width:768px) {
    .popup {
        display: none;
    }
}
</style>