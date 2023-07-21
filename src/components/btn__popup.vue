<template>
        <a href="#" class="menu-btn popup-link">
            <span></span>
            <span></span>
            <span></span>
        </a>
</template>>

<script>
export default {
    name: 'popupBtn'
}
</script>

<style>
    .menu-btn {
    display: block;
    width: 34px;
    height: 20px;
    position: relative;
    top: 55px;
    left: 90%;
    z-index: 2;
    overflow: hidden;
  }

  .menu-btn span {
    width: 37px;
    height: 4px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: #222222;
    transition: all 0.5s;
  }

  .menu-btn span:nth-of-type(2) {
    top: calc(50% - 8px);
  }

  .menu-btn span:nth-of-type(3) {
    top: calc(50% + 8px);
  }

  @media (min-width: 768px) {
    .menu-btn{ 
    display: none;
    }
  }
</style>>