<template>
  <section
    id="intro"
    class="py-16"
    :class="$vuetify.theme.dark ? 'black' : ' white'"
  >
    <v-container>
      <v-responsive class="max-auto mx-auto text-center" max-width="600">
        <h2 class="text-h4 text-md-h3 text-center font-weight-black mb-7">
          Welkom op mijn portfolio!
        </h2>
        <p class="title font-weight-light">
          Deze website heb ik gemaakt met mijn kennis van frontend development
          dat ik heb geleerd op <strong>Hogeschool PXL</strong>.
        </p>
      </v-responsive>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      cards: [
        {
          title: 'Best Productivity',
          subtitle: 'Professionally developed',
          text: 'All components and features are developed using the most up-to-date coding practices.',
          callout: '01',
        },
        {
          title: 'Fast & optimized',
          subtitle: 'Performance',
          text: 'Themes are designed for maximum performance and are semantically structured to maximize SEO.',
          callout: '02',
        },
        {
          title: 'Built on Vuetify',
          subtitle: 'Material Design',
          text: "Being developed with Vuetify means you have access to all of the framework's available features.",
          callout: '03',
        },
      ],
    }
  },
}
</script>
