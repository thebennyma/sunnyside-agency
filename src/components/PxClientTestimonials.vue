<template>
  <div class="container">
    <span class="container__tittle">CLIENT TESTIMONIALS</span>
    <div class="container__testimonials">
      <div
        class="container__testimonials__clients"
        v-for="(client, index) in clients"
        :key="index"
      >
        <img :src="require(`@/assets/clients/image-${client.img}.jpg`)" />
        <p>{{ client.comments }}</p>
        <div>
          <span class="name-client">{{ client.nameClient }}</span>
          <span class="tittle-client">{{ client.titleClient }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      clients: [
        {
          img: "emily",
          comments:
            "We put our turst in Sunnyside and they delivered, making sure our needs were met and deadlines wwere always hit.",
          nameClient: "Emily R.",
          titleClient: "Marketing Director",
        },
        {
          img: "thomas",
          comments:
            "Sunnyside's enthusiasm coupled with their keen interest in our brand's success made it a satisfying and enjoyable experience.",
          nameClient: "Thomas S.",
          titleClient: "Chief Operating Officer",
        },
        {
          img: "jennie",
          comments:
            "Incredible and result! Our sales increased over 400% when we worked with Sunnyside. Highly recommended!",
          nameClient: "Jenny F.",
          titleClient: "Business Owner",
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.container {
  display: grid;
  grid-row-gap: 8rem;
  padding: 6rem 2rem;
  &__tittle {
    font-size: 3rem;
    font-weight: 900;
  }
  &__testimonials {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    &__clients {
      display: grid;
      grid-row-gap: 3rem;
      justify-items: center;
      img {
        border-radius: 6rem;
      }
      p {
        width: 400px;
        font-size: 1.2rem;
        font-weight: bold;
        color: hsl(213, 9%, 39%);
      }
      div {
        display: grid;
        grid-row-gap: 0.5rem;
        width: 100%;
        .name-client {
          color: hsl(212, 27%, 19%);
          font-weight: 900;
        }
        .tittle-client {
          font-size: 14px;
          font-weight: bold;
          color: hsl(213, 9%, 39%);
        }
      }
    }
  }
}
@media only screen and (max-width: 1240px) {
  .container {
    grid-row-gap: 2rem;
    &__tittle {
      font-size: 2rem;
      font-weight: 900;
    }
    &__testimonials {
      grid-template-columns: 1fr;
      grid-row-gap: 5rem;
      padding: 3rem 0rem;
      &__clients {
        p {
          width: 400px;
          font-size: 1.2rem;
          font-weight: bold;
          color: hsl(213, 9%, 39%);
        }
      }
    }
  }
}
@media only screen and (max-width: 650px) {
  .container {
    &__testimonials {
      grid-template-columns: 1fr;
      grid-row-gap: 5rem;
      padding: 3rem 0rem;
      &__clients {
        p {
          width: 100%;
          font-size: 1.2rem;
          font-weight: bold;
          color: hsl(213, 9%, 39%);
        }
      }
    }
  }
}
</style>
