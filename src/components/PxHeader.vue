<template>
  <div class="container">
    <span>WE ARE CREATIVES</span
    ><img src="@/assets/header/image-header.jpg" class="desk" alt="" /><img
      src="@/assets/header/image-header-mobi.jpg"
      class="mobile"
      alt=""
    />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: grid;
  position: relative;
  .desk {
    display: flex;
    width: 100%;
    height: auto;
  }
  .mobile {
    display: none;
  }
  span {
    position: absolute;
    font-weight: 900;
    font-size: 3rem;
    color: #fff;
    top: 35%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
@media only screen and (max-width: 900px) {
  .container {
    span {
      position: absolute;
      font-weight: 900;
      font-size: 2rem;
      color: #fff;
      top: 20%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    .desk {
      display: none;
    }
    .mobile {
      display: flex;
      width: 100%;
      height: auto;
    }
  }
}
@media only screen and (max-width: 600px) {
  .container {
    span {
      position: absolute;
      font-weight: 900;
      font-size: 2rem;
      color: #fff;
      top: 30%;
      left: 50%;
      transform: translate(-50%, -50%);
    }
    .desk {
      display: none;
    }
    .mobile {
      display: flex;
      width: 100%;
      height: auto;
    }
  }
}
</style>
