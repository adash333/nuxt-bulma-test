<template>
  <section class="hero is-primary is-bold">
    <div class="hero-body">
      <h1 class="title is-size-2">
        About
      </h1>
      <h2 class="subtitle is-size-4">
        NBHとは？
      </h2>
    </div>
  </section>
  
  <div class="section">
    <div class="columns">
      <div class="column">
        <p class="bd-notification is-primary">First column</p>
      </div>
      <div class="column">
        <p class="bd-notification is-primary">Second column</p>
      </div>
      <div class="column">
        <p class="bd-notification is-primary">Third column</p>
      </div>
      <div class="column">
        <p class="bd-notification is-primary">Fourth column</p>
      </div>
    </div>
  </div>
    
</template>

<script>
export default {
  fetch ({store}) {
    store.commit('resetMenu')
  }
}
</script>
