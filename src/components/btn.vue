<template>
        <button class = "btn">
            <span class = "btn__text">Send message</span>
        </button>
</template>

<script>

export default ({
    name: 'btnFooter'
})
</script>
>
<style>
.btn {
    position: relative;
    font-family: "Roboto-Medium";
    border: 0;
    background-color: transparent;
    background-image: url('./icon/btn.svg');
    background-position: center;
    background-repeat: no-repeat;
    -webkit-tap-highlight-color: transparent;
    font-size: 18px;
    line-height: 1;
    display: flex;
    text-align: center;
    align-items: center;
    color: #ffffff;
    padding: 11px 96px 13px 96px;
    border-radius: 25px;
    overflow: hidden;
    margin: 0 auto;
  }
  
  .btn::before {
    content: '';
    display: block;
    position: absolute;
    left: 0;
    top: 0;
    height: 100%;
    background-color: #000;
  }

  @media (min-width: 500px){
    .btn{
        padding: 11px 29px 13px 29px;
        margin-top: 12%;
    }
  }
</style>>