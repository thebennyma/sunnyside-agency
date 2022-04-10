<template>
  <div class="home">
    <PxHeaderMenu />
    <PxHeader />
    <PxTransformBrand />
    <PxStandOutRightAudience />
    <PxPhotographyGraphicDesing />
    <PxClientTestimonials />
    <PxImageGallery />
    <PxFooter />
  </div>
</template>

<script>
import PxHeaderMenu from "@/components/PxHeaderMenu.vue";
import PxHeader from "@/components/PxHeader.vue";
import PxTransformBrand from "@/components/PxTransformBrand.vue";
import PxStandOutRightAudience from "@/components/PxStandOutRightAudience.vue";
import PxPhotographyGraphicDesing from "@/components/PxPhotographyGraphicDesing.vue";
import PxClientTestimonials from "@/components/PxClientTestimonials.vue";
import PxImageGallery from "@/components/PxImageGallery.vue";
import PxFooter from "@/components/PxFooter.vue";

export default {
  name: "HomeView",
  components: {
    PxHeaderMenu,
    PxHeader,
    PxTransformBrand,
    PxStandOutRightAudience,
    PxPhotographyGraphicDesing,
    PxClientTestimonials,
    PxImageGallery,
    PxFooter,
  },
};
</script>
