<script setup>
import Header from './components/Header.vue'
import Footer from './components/Footer.vue'
import productInfo from './assets/data.json'
import Details from './components/Details.vue'
</script>

<template>
  <Header />

  <main>
    <div class="container">
      <div></div>
      <Details />
    </div>
  </main>

  <Footer />
</template>

<style scoped>
.constainer {
  display: flex;
}

.container > div:last-child {
  padding: 25px 0 25px 100px;
}

h1 + p {
  font-size: 22px;
  margin-bottom: 25px;
}

h1 + p span {
  color: #66676e;
  font-size: 14px;
  font-weight: lighter;
}

.container {
  display: flex;
  height: calc(
    100vh - var(--header-top-height) - var(--header-bottom-height) - var(--footer-height)
  );
  border: solid green;
}

.container > div {
  border: 1px solid;
  width: 50%;
}

.rate {
  margin-bottom: 40px;
}

.rate svg {
  margin-right: 3px;
}

.advise {
  background-color: #efeff0;
  padding: 20px;
  font-size: 14px;
  line-height: 20px;
  font-weight: lighter;
  margin-bottom: 10px;
}

.cart-bloc {
  display: flex;
  gap: 10px;
}

.cart-bloc button {
  font-family: inherit;
  font-size: inherit;
  font-weight: bold;
  background-color: var(--main-black);
  color: white;
  flex: 1;
  border: none;
  cursor: pointer;
}

.cart-bloc button:hover {
  opacity: 0.7;
}

.cart-bloc div {
  width: 50px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid var(--main-black);
  color: var(--main-black);
}

.cart-bloc div:hover {
  border-width: 3px;
}

.cart-bloc svg {
  width: 25px;
  height: 25px;
  cursor: pointer;
}
</style>
