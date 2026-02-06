<script setup>

</script>

<template>
  <div :class="$style.header">
    <div :class="$style.logoBurger">
      <div :class="$style.logo">LOGO</div>
      <img :class="$style.button" src="../assets/icons/burger.svg" alt="" />
    </div>
    <div :class="$style.wrapperLogo">
      <div :class="$style.text">Искать жильё</div>
      <div :class="$style.text">Блог</div>
      <div :class="$style.text">Частые вопросы</div>
      <img
        :class="$style.icon"
        width="24"
        height="24"
        src="@/assets/icons/bell.svg"
        alt="bell"
      />
      <img
        :class="$style.icon"
        width="24"
        height="24"
        src="@/assets/icons/like.svg"
        alt="like"
      />
      <div :class="$style.bigTxt">Мой аккаунт</div>
    </div>
  </div>
</template>

<style  module  lang="scss" >

.header{
  max-width: 64rem;
  margin: 0 auto 1.375rem;
  display: flex;
  justify-content: space-between;
  padding: 1rem 1.5rem;
  border-bottom: 1px solid $bottom-border;

  @media (max-width: 832px) {
    margin: 0 0 2.875rem 0;
  }

  .logoBurger {
    display: flex;

    @media (max-width: 832px) {
      width: 100%;
      justify-content: space-between;
      gap: 4.5rem;
    }

    .logo {
      width: 13.75rem;
      height: 3.5rem;
      background: $background-color;

      @media (max-width: 432px) {
        min-width: 10.25rem;
        height: 3.25rem;
      }
    }

  

    .button {
      padding: 0.875rem;
      border: 1px solid $black-txt;
      border-radius: 0.5rem;
      cursor: pointer;
display: none;
      @media (max-width: 832px) {
        display: block;
      }
    }
  }

  .wrapperLogo {
    display: flex;
    justify-content: space-between;
    gap: 1rem;
    align-items: center;

    @media (max-width: 832px) {
      display: none;
    }

    .text {
      color: $grey-txt;
      font-size: 1rem;
      cursor: pointer;

      &:hover {
        color: $blue-txt;
        cursor: pointer;
        transition: color 0.3s ease-in-out;
      }
    }

    .bigTxt {
      padding: 0.875rem 1.5rem;
      border: 1px solid $black-txt;
      color: $black-txt;
      border-radius: 0.5rem;
      cursor: pointer;

      &:hover{
        color: $blue-txt;
        transition: color 0.3s ease-in-out;
      }
    }
  }
}

</style>
