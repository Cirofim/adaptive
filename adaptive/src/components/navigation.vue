<script></script>

<template>
  <div :class="$style.bottomWr">
    <div :class="$style.navigationWr">
      <a href="" :class="$style.linkWr">
        <div :class="$style.textNav">Посуточная аренда</div>
      </a>
      <div :class="$style.trait">/</div>
      <a href="" :class="$style.linkWr">
        <div :class="$style.textNav">Барановичи, Брестская область</div>
      </a>
      <div :class="$style.trait">/</div>
      <a href="" :class="$style.linkWr">
        <div :class="$style.textNav">70 - 150 BYN</div>
      </a>
      <div :class="$style.trait">/</div>
      <a href="" :class="$style.linkWr">
        <div :class="$style.textNav">27.09.25 - 30.09.25</div>
      </a>
    </div>
    <div :class="$style.wrapperRight">
      <div :class="$style.textPn">Сохранить вариант</div>
      <img :class="$style.grey_like" src="@/assets/icons/grey_like.svg" alt="" />
    </div>
  </div>
</template>

<style module lang="scss">

.bottomWr {
  max-width: 64rem;
  margin: 0 auto;
  padding: 0 0 0 1.5rem;
  display: flex;
  gap: 0.75rem;

  @media (max-width: 1024px) {
    flex-wrap: wrap;
    padding: 0;
  }

  .navigationWr {
    display: flex;

    .linkWr {
      display: flex;

      .textNav {
        font-size: 1rem;
        padding: 0.375rem 0.875rem 0.375rem 0.875rem;
        white-space: nowrap;
        color: $grey-txt;

        .textNav {
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

  .wrapperRight {
    display: flex;
    gap: 8px;
    padding: 0.375rem 0.875rem;
    cursor: pointer;
    color: $grey-txt;

    .textPn {
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
