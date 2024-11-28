<script setup>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
</script>

<template>
  <header>
    <div class="headerTop">
      <div class="container">
        <p>Essayez d'abord, <span>payez après</span></p>
        <p>LIVRAISON & RETOUR <span>GRATUITS*</span></p>
        <p>Retour et remboursements</p>
      </div>
    </div>

    <div class="headerBottom">
      <div class="container">
        <nav>
          <a>Femme</a>
          <a>Homme</a>
          <a>Enfant</a>
        </nav>

        <img src="../assets/img/logo.svg" />

        <nav>
          <FontAwesomeIcon :icon="['far', 'user']" />
          <FontAwesomeIcon :icon="['far', 'heart']" />
          <FontAwesomeIcon :icon="['fas', 'shopping-bag']" />
        </nav>
      </div>
    </div>
  </header>
</template>

<style scoped>
/* HEADER TOP */
.headerTop {
  background-color: var(--light-grey);
}

.headerTop .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: var(--header-top-height);
  color: var(--dark-grey);
  font-size: 12px;
}

span {
  color: var(--main-orange);
}

svg {
  color: var(--main-black);
  padding: 10px;
  border: 2px solid white;
}

svg:hover{
  border:2px solid black
}

/* HEADER BOTTOM */
.headerBottom {
  border-bottom: 1px solid var(--light-grey);
}

.headerBottom .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: var(--header-bottom-height);
}

a {
  color: inherit;
  font-weight: bold;
  padding: 10px 15px;
}

a:first-child {
  background-color: var(--main-black);
  color: white;
}

img {
  width: 155px;
}

nav {
  display: flex;
  gap: 10px;

  flex: 1;
}

nav:last-of-type {
  justify-content: flex-end;
}
</style>
