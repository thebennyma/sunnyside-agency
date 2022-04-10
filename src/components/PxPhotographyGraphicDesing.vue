<template>
  <div class="container">
    <div class="container__graphic-desing">
      <img src="@/assets/food/image-graphic-design.jpg" alt="" />
      <div>
        <span>Graphic Desing</span>
        <p>
          Grat design makes you memorable. We deliver artwork that underscores
          your brand message and captures potential clients attention.
        </p>
      </div>
    </div>
    <div class="container__photography">
      <img src="@/assets/food/image-photography.jpg" alt="" />
      <div>
        <span>Photography</span>
        <p>
          Increase your credibility by getting the most stunning, high-quality
          photos that improve your business image.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  &__photography,
  &__graphic-desing {
    position: relative;
    img {
      display: flex;
      width: 100%;
      height: auto;
    }
    div {
      display: grid;
      grid-row-gap: 2rem;
      position: absolute;
      top: 80%;
      left: 50%;
      transform: translate(-50%, -50%);
      span {
        font-size: 1.5rem;
        font-weight: 900;
      }
      p {
        font-weight: bold;
        line-height: 1.5rem;
      }
    }
  }
  &__photography {
    div {
      color: hsl(198, 62%, 26%);
    }
  }
  &__graphic-desing {
    div {
      color: hsl(167, 40%, 24%);
    }
  }
}
@media only screen and (max-width: 1120px) {
  .container {
    grid-template-columns: 1fr 1fr;
    &__photography,
    &__graphic-desing {
      div {
        grid-row-gap: 1.5rem;
        top: 75%;
        span {
          font-size: 1.2rem;
        }
      }
    }
  }
}
@media only screen and (max-width: 870px) {
  .container {
    grid-template-columns: 1fr;
    &__photography,
    &__graphic-desing {
      div {
        grid-row-gap: 1.5rem;
        top: 75%;
        span {
          font-size: 1.2rem;
        }
      }
    }
  }
}
@media only screen and (max-width: 475px) {
  .container {
    &__photography,
    &__graphic-desing {
      div {
        width: 80%;
        grid-row-gap: 1rem;
        top: 75%;
        span {
          font-size: 1rem;
        }
        p {
          font-size: 0.8rem;
        }
      }
    }
  }
}
</style>
