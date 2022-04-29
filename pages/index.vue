<template>
  <section id="home">
    <v-row no-gutters>
      <v-col cols="12">
        <!-- CAROUSEL -->
        <SectionsHero id="carousel" />

        <!-- WELKOM INTRO -->
        <SectionsIntro id="intro" />

        <!-- VOORSTELLING -->
        <SectionsTestimonials id="voorstelling" />

        <!-- ACTIVITEITEN -->
        <SectionsFeatures id="activiteiten" />

        <!-- ACTIVITEITEN -->
        <reflectieverslagen id="reflectieverslagen" />

        <!-- ACTIVITEITEN -->
        <eindreflectie id="eindreflectie" />
      </v-col>
    </v-row>
  </section>
</template>

<script>
import Eindreflectie from '~/components/sections/Eindreflectie.vue'
import reflectieverslagen from '~/components/sections/reflectieverslagen.vue'
export default {
  components: { Eindreflectie, reflectieverslagen },
  data() {
    return {
      //
    }
  },
}
</script>
