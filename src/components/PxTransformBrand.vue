<template>
  <div class="container">
    <div class="container__information">
      <span>Transform your brand</span>
      <p>
        We are a full-service creative agency specializaing in helping brands
        grow fast. Engage your clients through compelling visuals that do most
        of the marketing for you.
      </p>
      <a>LEARN MORE</a>
    </div>
    <img
      class="container__image"
      src="@/assets/food/image-transform.jpg"
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
  grid-template-columns: 1fr 1fr;

  &__image {
    width: 100%;
    height: auto;
  }
  &__information {
    display: grid;
    grid-row-gap: 4rem;
    text-align: left;
    padding: 4rem 10% 4rem 10%;
    align-self: center;
    span {
      font-size: 2.5rem;
      font-weight: 900;
    }
    p {
      font-size: 1.3rem;
      color: hsl(232, 10%, 55%);
    }
    a {
      font-size: 1.6rem;
      font-weight: bold;
      cursor: pointer;
    }
    p,
    a {
      font-family: "Outfit", sans-serif;
      font-family: "Space Mono", monospace;
    }
  }
}
@media only screen and (max-width: 1181px) {
  .container {
    &__image {
    }
    &__information {
      grid-row-gap: 2rem;
      padding: 4rem;
    }
  }
}
@media only screen and (max-width: 1120px) {
  .container {
    &__information {
      grid-row-gap: 3rem;
      padding: 4rem;
      span {
        font-size: 2rem;
      }
      p {
        font-size: 1rem;
      }
      a {
        font-size: 1.2rem;
      }
    }
  }
}
@media only screen and (max-width: 1000px) {
  .container {
    &__information {
      grid-row-gap: 1rem;
      padding: 4rem;
      span {
        font-size: 2rem;
      }
      p {
        font-size: 1rem;
      }
      a {
        font-size: 1.2rem;
      }
    }
  }
}

@media only screen and (max-width: 920px) {
  .container {
    grid-template-columns: 1fr;
    grid-template-areas: "image" "information";
    &__imgage {
      grid-area: image;
    }
    &__information {
      grid-area: information;
      text-align: center;
    }
  }
}
@media only screen and (max-width: 600px) {
  .container {
    &__information {
      grid-row-gap: 2rem;
      padding: 3rem;
    }
  }
}
</style>
