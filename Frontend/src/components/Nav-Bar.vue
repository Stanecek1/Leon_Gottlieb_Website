<template>
    <vue-navigation-bar  :options="navbarOptions" />
</template>
  
  <script>
//   import brandImage from '../src/assets/images/lockup-color.png'
  
  export default {
      data() {
        return {
          navbarOptions: {
            class: "navigation-body",
            elementId: "main-navbar",
            isUsingVueRouter: true,
            ariaLabelMainNav: "Main Navigation",
            tooltipAnimationType: "shift-away",
            tooltipPlacement: "bottom",
            background:'#000000',
            menuOptionsRight: [
            {
                type: "link",
                text: "home",
                path: { name: "home"},
            },
            {
                type: "link",
                text: "books",
                path: { name: "books"},
            },
            {
                type: "link",
                text: "about",
                path: { name: "about"},
            },
            {
                type: "link",
                text: "contact",
                path: { name: "contact"},
            },
            {
                type: "link",
                text: "excerpts",
                path: { name: "excerpts"},
            },
            ],
          }
        }
      }
  }
  </script>
  
  <style lang="scss">
    .vnb {
        font-family: matesc;
        display: grid;
        justify-content: top;
        background: rgb(245, 245, 245) !important;
        height: 5vh;
        border-bottom: solid black 1px;

      }
    .vnb a {
      color: black;
      font-size: large;
    }
    .vnb__menu-options{
      padding-left: 0;
    }
    .vnb__menu-options .vnb__menu-options--left{
      padding-left: 0;
    }
    .vnb__brand-image-wrapper{
      display: none;
    }
    .vnb__menu-options--left{
      display: none !important;
    }

    
  </style>