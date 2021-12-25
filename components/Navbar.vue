<template>
  <div class="navbar">
    <div class="logo-wrapper">
      <img src="@/assets/images/logo.png" alt="" />
      <div class="logo-text">
        <h4>Skilline</h4>
      </div>
    </div>
    <div class="navbar-links">
      <a href="">Home</a>
      <a href="">Carrers</a>
      <a href="">Blog</a>
      <a href="">About Us</a>
      <div class="navbar-reg">
        <a class="log right" href="">Log in</a>
        <a class="log" href="">Sign Up</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.navbar {
  display: flex;
  align-items: center;
  justify-content: space-between;

  .logo-wrapper {
    position: relative;

    .logo-text {
      position: absolute;
      top: 15%;
      left: 40%;

      h4 {
        font-family: Popp;
        font-style: normal;
        font-weight: 700;
        font-size: 32px;
        color: #113c49;
      }
    }
  }

  &-links {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 70%;

    a {
      font-family: Popp;
      font-style: normal;
      font-weight: normal;
      font-size: 22px;
      color: #252641;
      text-decoration: none;
      transition: 0.3s all;

      &:hover {
        transform: translateY(-10px);
      }
    }

    .navbar-reg {
      .log {
        border: 1px solid #ffffff;
        background: #ffffff;
        box-shadow: 0px 20px 24px rgba(0, 0, 0, 0.03);
        border-radius: 80px;
        padding: 10px 40px;

        &.right {
          margin-right: 35px;
        }

        &:hover {
          background: #f48c06;
          color: #ffffff;
        }
      }
    }
  }
}
</style>
