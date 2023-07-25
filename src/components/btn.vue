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
    font-family: "Roboto";
    font-weight: 500;
    border: 0;
    background-color: transparent;
    background-color: #000;
    background-position: center;
    background-repeat: no-repeat;
    -webkit-tap-highlight-color: transparent;
    font-size: 18px;
    line-height: 1;
    display: flex;
    text-align: center;
    align-items: center;
    color: #ffffff;
    padding: 12px 95px 12px 95px;
    border-radius: 25px;
    overflow: hidden;
    margin: 0 auto;
  }
  
  @media (min-width: 500px){
    .btn{
        padding: 12px 30px 12px 30px;
        margin-top: 30px;
    }
  }
</style>>