<template>
  <div class="main_wrap">
    <NavbarComp/>
    <HeroComp/>
    <FeaturesComp/>
    <TestimonialsComp/>
    <CtaComp/>
    <FooterComp/>
  </div>
</template>

<script>
import NavbarComp from '@/components/NavbarComp.vue'
import HeroComp from '@/components/HeroComp.vue'
import FeaturesComp from '@/components/FeaturesComp.vue'
import TestimonialsComp from '@/components/TestimonialsComp.vue'
import CtaComp from '@/components/CtaComp.vue'
import FooterComp from '@/components/FooterComp.vue'
export default {
  components: {
    NavbarComp,
    HeroComp,
    FeaturesComp,
    TestimonialsComp,
    CtaComp,
    FooterComp
  }
}
</script>

<style>
.main_wrap {
  background-image: url('@/assets/img/bg-tablet-pattern.svg');
  background-repeat: no-repeat;
  background-size: 800px;
  background-position: 90% -25%;
}
@media(max-width: 576px) {
  .main_wrap {
    background-position: 50px -50px;
    background-size: 500px;
  }
}
</style>