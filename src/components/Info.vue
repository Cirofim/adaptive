<script setup></script>

<template>

  <div :class="$style.container">
    <div :class="$style.wrapper">
      <p :class="$style.blue">Новое предложение</p>
      <p :class="$style.address">Комсомольская ул, 21, Барановичи, Брестская область</p>
      <div :class="$style.icons">
        <div :class="$style.icon">
          <img src="@/assets/icons/icon-room.svg" alt="" />
          <div :class="$style.house">2 комн.</div>
        </div>
        <div :class="$style.icon">
          <img src="@/assets/icons/icon-meters.svg" alt="" />
          <div :class="$style.house">52 м²</div>
        </div>
        <div :class="$style.icon">
          <img src="@/assets/icons/icon-floor.svg" alt="" />
          <div :class="$style.house">3 этаж</div>
        </div>
      </div>
      <div :class="$style.services">
        <p :class="$style.facilities">Основные удобства</p>
        <div :class="$style.description">
          <div :class="$style.texxt">Бесплатный Wi-Fi</div>
          <div :class="$style.texxt">Телевизор</div>
          <div :class="$style.texxt">Кондиционер</div>
          <div :class="$style.texxt">Рабочая зона</div>
          <div :class="$style.texxt">Фен</div>
          <div :class="$style.texxt">Душквая кабина</div>
          <div :class="$style.texxt">Вмд из окна</div>
          <div :class="$style.texxt">Комплект полотенец</div>
          <div :class="$style.texxt">Водонагреватель</div>
          <div :class="$style.texxt">Утюг</div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" module>
.container {
  .wrapper{
    max-width: 40.125rem;
    margin: 0 1.5rem;

    .blue{
      font-size: 1rem;
      color: $blue-text-info;
      background: $background-text-blue;
      display: inline-block;
      margin: 0 0 1.5rem 0;
      font-weight: 400;
      padding: 0.125rem 0.5rem;
    }

    .address{
      font-size: 1rem;
      font-weight: 400;
      margin: 0 0 1.5rem 0;
    }

    .icons{
      display: flex;
      align-items: center;
      gap: 1.5rem;
      margin: 0 0 1.5rem 0;
      @media(max-width:390px){
        flex-wrap: wrap;
      }

      .icon{
        display: flex;
        gap: 0.5rem;

        .house{
          padding:  0.5rem 0;
          font-size: 1.125rem;
          font-weight: 500;
        }

        img{
          background: $background-color;
          border-radius: 0.625rem;
          padding: 0.25rem;
          width: 2.125rem;
          height: 2.125rem;
        }
      }
    }
  }
.services{
  .facilities{
    font-size: 1.125rem;
    color: $black-text;
    font-weight: 500;
  }
  .description{
    display: flex;
    flex-wrap: wrap;
    gap: 1rem 1rem;

    @media(max-width:690px){
 
      flex-wrap: wrap;
    }
    .texxt{
      padding: 0.125rem 0.5rem;
      background: $background-color;
      border-radius: 0.375rem;
      font-weight: 400;
    }

  }
}

}
</style>
