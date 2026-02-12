<script setup></script>

<template>
  <div :class="$style.container">
    <div :class="$style.wrapper">
      <div :class="$style.big">
        <img src="@/assets/img/house.png" alt="" />
      </div>

      <div :class="$style.small">
        <img src="@/assets/img/house(2).png" alt="" />
      </div>

      <div :class="$style.small">
        <img src="@/assets/img/house(3).png" alt="" />
      </div>

      <div :class="$style.button">
        <div :class="$style.text">Показать все фото</div>
        <img :class="$style.icon" src="@/assets/icons/image.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss" module>
.container {
  display: flex;
  flex-wrap: wrap;
  margin: 0 0 1.75rem 0;

  .wrapper {
    max-width: 64rem;
    position: relative;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1.5rem 1.625rem;

    img {
      @media (max-width: 900px) {
        width: 20rem;
        height: 14.75rem;
      }
    }

    @media (max-width: 900px) {
      height: 15rem;
      display: flex;
      gap: 0.5rem;
      overflow-x: auto;
      scroll-snap-type: x mandatory;
    }

    .big {
      grid-column: 1/2;
      grid-row: 1/3;
      scroll-snap-align: start;

      @media (max-width: 900px) {
        width: 20rem;
        height: 14.75rem;
      }
    }

    .small {
      @media (max-width: 900px) {
        scroll-snap-align: start;
        width: 20rem;
        height: 14.75rem;
      }
    }
  }

  .button {
    padding: 0.875rem 1.5rem;
    display: flex;
    gap: 0.5rem;
    background: $button-photo;
    position: absolute;
    bottom: 1.125rem;
    right: 1.5rem;
    z-index: 2;
    border-radius: 0.5rem;

    &:hover {
      color: $blue-txt;
      transition: color 0.3s ease-in-out;
      cursor: pointer;
    }

    @media (max-width: 900px) {
      display: none;
    }
  }
}
</style>
