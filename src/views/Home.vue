<template>
  <div class="home">
    <header class="header">
      <div class="header__container">
       <Logo/>
       <input class="search" type="text" placeholder="Пошук">
       <div class="cart">
         <cart-icon/>
       </div>
      </div>
    </header>
    <main>
      <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Commodi, est et libero necessitatibus neque quo reiciendis similique! Atque deserunt dolorem exercitationem molestias quisquam, sed suscipit voluptas? Doloremque eum magnam minima.</p>
    </main>
  </div>
</template>

<script>
import Logo from "../assets/logo"
import cartIcon from "../assets/cart-icon"

export default {
  name: 'Home',
  components: {
    Logo,
    cartIcon
  }
}
</script>
<style lang="scss">
.header {
  background: white;
  &__container {
    display: flex;
    justify-content: space-between;
  }
  .search {
    padding: 0 15px;
    border: 1px solid #E5EAEF;
    border-radius: 30px;
    max-width: 120px;
    background-image: url("../assets/search.svg");
    background-position: right;
    background-size: 20px;
    background-repeat: no-repeat;
  }
}
.cart {
  width: 44px;
  height: 44px;
  background: #3985C6;
  border-radius: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
