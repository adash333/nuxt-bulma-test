<template>
  <nav class="navbar is-white" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <div class="navbar-item">Nuxt Bulma Hamburger2</div>
      <div class="navbar-burger" 
        data-target="navMenu" 
        @click="$store.commit('toggleMenu')" 
        :class="{'is-active': $store.state.isMenuActive}">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div><!-- navbar-brand END -->
    <div class="navbar-menu" 
      id="navMenu" 
      :class="{'is-active': $store.state.isMenuActive}">
      <div class="navbar-start">
        <nuxt-link to="/" class="navbar-item">HOME</nuxt-link>
        <nuxt-link to="/about" class="navbar-item">NBHとは？</nuxt-link>
        <nuxt-link to="/contact" class="navbar-item">お問い合わせ</nuxt-link>
      </div> 
      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <a class="button is-primary">
              <strong>Sign up</strong>
            </a>
            <a class="button is-light">
              Log in
            </a>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>