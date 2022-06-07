<template>
  <div class="navbar">
    <div class="container">
      <div class="navbar-wrapper">
        <div class="navbar-wrapper__image">
          <img src="@/assets/img/Logo.png" alt="" />
        </div>
        <div class="navbar-card-wrapper">
          <NavbarCard />
        </div>
        <div class="navbar-wrapper__item">
          <div class="navbar-wrapper__subtitle">Sign in</div>
          <div class="navbar-wrapper__btn">
            <button class="navbar-btn">Get started</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import NavbarCard from "@/components/NavbarCard";
export default {
  name: "Navbar",
  components: {
    NavbarCard,
  },
};
</script>

<style lang="scss" scoped>
.navbar {
  padding: 50px 0px;
}
.navbar-wrapper {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.navbar-wrapper__item {
  display: flex;
  gap: 30px;
  .navbar-btn {
    color: white;
    background-color: #0075ff;
    border-radius: 5px;
    border: none;
    cursor: pointer;
    padding: 5px 20px;
  }
}
.navbar-wrapper__image img {
  width: 100%;
}
@media screen and (max-width: 1200px) {
  .navbar-wrapper__item {
    gap: 20px;
  }
}
@media screen and (max-width: 768px) {
  .navbar-wrapper__item {
    display: flex;
    flex-direction: column;
    gap: 5px;
  }
  .navbar-wrapper {
    display: flex;
    flex-direction: column;
    gap: 30px;
    text-align: center;
  }
}
@media screen and (max-width: 576px) {
  .navbar-wrapper {
    gap: 20px;
  }
}
</style>
