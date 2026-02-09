<script></script>

<template>
  <div :class="$style.wrapper">
    <div :class="$style.navigationWr">
      <a href="" :class="$style.link">
        <div :class="$style.text">Посуточная аренда</div>
      </a>
      <div :class="$style.trait">/</div>
      <a href="" :class="$style.link">
        <div :class="$style.text">Барановичи, Брестская область</div>
      </a>
      <div :class="$style.trait">/</div>
      <a href="" :class="$style.link">
        <div :class="$style.text">70 - 150 BYN</div>
      </a>
      <div :class="$style.trait">/</div>
      <a href="" :class="$style.link">
        <div :class="$style.text">27.09.25 - 30.09.25</div>
      </a>
    </div>
    <div :class="$style.right">
      <div :class="$style.pn">Сохранить вариант</div>
      <img :class="$style.grey" src="@/assets/icons/grey-like.svg" alt="" />
    </div>
  </div>
</template>

<style lang="scss" module>
.wrapper {
  margin: 0 auto 1.375rem;
  padding: 0 0 0 1.5rem;
  display: flex;
  gap: 0.75rem;

  @media (max-width: 1024px) {
    flex-wrap: wrap;
    padding: 0;
  }

  .navigationWr {
    display: flex;

    .link {
      display: flex;

      .text {
        font-size: 1rem;
        padding: 0.375rem 0.875rem 0.375rem 0.875rem;
        white-space: nowrap;
        color: $grey-txt;

        .text {
          padding: 0.375rem 0.625rem 0.375rem 0;
        }

        &:hover {
          color: $blue-txt;
          cursor: pointer;
          transition: color 0.3s ease-in-out;
        }

        @media (max-width: 830px) {
          padding: 0.375rem 0.875rem 0.375rem 0;
        }
      }
    }

    @media (max-width: 768px) {
      flex-wrap: wrap;
    }

    .trait {
      padding: 0.375rem 0;
      color: $grey-txt;

      @media (max-width: 830px) {
        padding: 0.375rem 0.875rem 0.375rem 0;
      }
    }
  }

  .right {
    display: flex;
    gap: 8px;
    padding: 0.375rem 0.875rem;
    cursor: pointer;
    color: $grey-txt;

    .pn {
      padding: 0;
    }

    @media (max-width: 830px) {
      padding: 0.375rem 0.875rem 0.375rem 0;
    }

    &:hover {
      color: $blue-txt;
      transition: color 0.3s ease-in-out;
    }
  }
}
</style>
