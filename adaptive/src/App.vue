<script></script>
<template>
  <header>
    <div class="header_container">
      <div class="wrapper_logo-burger">
        <div class="logo">LOGO</div>
        <img class="burger_button" src="./assets/icons/burger.svg" alt="" />
      </div>
      <div class="wrapper_logo">
        <div class="logo_text">Искать жильё</div>
        <div class="logo_text">Блог</div>
        <div class="logo_text">Частые вопросы</div>
        <img
          class="icon_logo"
          width="24"
          height="24"
          src="@/assets/icons/bell.svg"
          alt="bell"
        />
        <img
          class="icon_logo"
          width="24"
          height="24"
          src="@/assets/icons/like.svg"
          alt="like"
        />
        <div class="logo_text big_text">Мой аккаунт</div>
      </div>
    </div>

    <div class="wrapper_bottom">
      <div class="wrapper_navigation">
        <a href="" class="wrapper_link-navigation">
          <div class="navigation_text padding-text--left">
            Посуточная аренда
          </div>
        </a>
        <div class="navigation_text trait_text">/</div>
        <a href="" class="wrapper_link-navigation">
          <div class="navigation_text">Барановичи, Брестская область</div>
        </a>
        <div class="navigation_text trait_text">/</div>
        <a href="" class="wrapper_link-navigation">
          <div class="navigation_text">70 - 150 BYN</div>
        </a>
        <div class="navigation_text trait_text">/</div>
        <a href="" class="wrapper_link-navigation">
          <div class="navigation_text">27.09.25 - 30.09.25</div>
        </a>
      </div>
      <div class="wrapper_navigation-bottom">
        <div class="navigation_text padding-none">Сохранить вариант</div>
        <img class="grey_like" src="@/assets/icons/grey_like.svg" alt="" />
      </div>
    </div>
  </header>
</template>

<style>
@import url(./assets/blocks/logo.css);
@import url(./assets/global/style.css);
@import url(./assets/blocks/navigation.css);
</style>
