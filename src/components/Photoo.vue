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
 
  

  @media(max-width:900px){
    left: -92px;
  }
 

  .upWrapp {
    position: relative;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px 26px;
    overflow: visible;
    min-width: none;
    

    @media (max-width: 900px) {
     
      gap: 16px;
      position: absolute;
      display: flex;
      
    }

    .bigImg {
      grid-column: 1/2;
      grid-row: 1/3;

      @media (max-width: 900px) {
        min-width: 584px;
        height: 320px0;
        flex-shrink: 0;
        max-width: none;
        
      }
    }

    .firstSmall {
      @media (max-width: 900px) {
        min-width: 584px;
        flex-shrink: 0;
        max-width: none;
      }
    }
    .secondSmall {
      @media (max-width: 900px) {
        min-width: 584px;
        flex-shrink: 0;
        max-width: none;
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
