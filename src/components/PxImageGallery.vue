<template>
  <div class="container">
    <img src="@/assets/ImageGallery/image-gallery-milkbottles.jpg" alt="" />
    <img src="@/assets/ImageGallery/image-gallery-orange.jpg" alt="" />
    <img src="@/assets/ImageGallery/image-gallery-cone.jpg" alt="" />
    <img src="@/assets/ImageGallery/image-gallery-sugarcubes.jpg" alt="" />
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.container {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr 1fr;
  img {
    width: 100%;
    height: auto;
  }
}
@media only screen and (max-width: 800px) {
  .container {
    grid-template-columns: 1fr 1fr;
  }
}
</style>
