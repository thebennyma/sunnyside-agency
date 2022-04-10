<template>
  <div class="container">
    <div class="container__information">
      <span class="container__information__title">sunnyside</span>
      <div class="container__information__links">
        <a>About</a>
        <a>Services</a>
        <a>Projets</a>
      </div>
    </div>
    <div class="container__social-media">
      <a href="https://www.facebook.com/" target="_blank"
        ><img src="@/assets/mediasocial/icon-facebook.svg"
      /></a>
      <a href="https://www.instagram.com/" target="_blank"
        ><img src="@/assets/mediasocial/icon-instagram.svg"
      /></a>
      <a href="https://twitter.com/" target="_blank"
        ><img src="@/assets/mediasocial/icon-twitter.svg"
      /></a>
      <a href="https://www.pinterest.com.mx/" target="_blank"
        ><img src="@/assets/mediasocial/icon-pinterest.svg"
      /></a>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: grid;
  grid-row-gap: 4rem;
  background: hsl(168, 74%, 71%);
  padding: 6rem;
  &__information {
    display: grid;
    grid-row-gap: 2rem;
    color: hsl(168, 34%, 41%);
    &__title {
      font-size: 2.5rem;
      font-weight: 900;
    }
    &__links {
      a {
        padding: 0rem 2rem;
        font-weight: bold;
        cursor: pointer;
      }
    }
  }
  &__social-media {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    width: 200px;
    justify-self: center;
    align-items: center;
  }
}
@media only screen and (max-width: 650px) {
  .container {
    padding: 6rem 0rem;
    &__information {
      &__links {
        a {
          padding: 0rem 1rem;
        }
      }
    }
  }
}
</style>
