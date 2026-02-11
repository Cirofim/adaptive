<script setup></script>

<template>
  <div :class="$style.containerImg">
    <div :class="$style.upWrapp">
      <img :class="$style.bigImg" src="../assets/img/house.png" alt="" />
      <img :class="$style.firstSmall" src="../assets/img/house(2).png" alt="" />
      <img
        :class="$style.secondSmall"
        src="../assets/img/house(3).png"
        alt=""
      />
      <div :class="$style.wrapperBtn">
        <div :class="$style.textBtn">Показать все фото</div>
        <img :class="$style.iconBtn" src="../assets/icons/image.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" module>
.containerImg {
 display: flex;
 flex-wrap: wrap;
  

  @media(max-width:900px){

  }
 

  .upWrapp {
    width: 64rem;
    position: relative;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px 26px;
   

    @media (max-width: 900px) {
     position: fixed;
     display: flex;
     gap: 0.5rem;
     overflow-x: scroll;
     scroll-snap-type: x mandatory;
    }

    .bigImg {
      grid-column: 1/2;
      grid-row: 1/3;

      @media (max-width: 900px) {
        width: 320px;
        height: 236px;
        scroll-snap-align: center;
        max-width: none;
        
      }
    }

    .firstSmall {
      @media (max-width: 900px) {
        
        width: 320px;
        height: 236px;
        max-width: none;
       scroll-snap-align: center;
      }
    }
    .secondSmall {
      @media (max-width: 900px) {
        width: 320px;
        height: 236px;
        max-width: none;
       scroll-snap-align: center;
      }
    }
  }

  .wrapperBtn {
    padding: 14px 24px;
    display: flex;
    gap: 0.5rem;
    background: #ffffffcc;
    position: absolute;
    bottom: 18px;
    right: 24px;
    z-index: 2;
    border-radius: 0.5rem;

    @media (max-width: 900px) {
      display: none;
    }
  }
}
</style>
