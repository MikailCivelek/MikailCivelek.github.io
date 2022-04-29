<template>
  <section class="py-16" :class="$vuetify.theme.dark ? 'black' : ' white'">
    <v-container>
      <v-row>
        <v-col class="text-center">
          <h2 class="text-h4 text-md-h3 text-center font-weight-black">
            Reflectieverslagen
          </h2>
          <br />
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(card, index) in cards"
          :key="index"
          cols="12"
          sm="4"
          class="text-center d-flex flex-column"
          ><NuxtLink :to="pages[index]">
            <v-sheet
              class="py-12 px-6 m-3 justify-center d-flex flex-column"
              style="
                margin: 0 auto;
                min-height: 500px;
                align-items: center;
                cursor: pointer;
              "
              :style="
                hover[index]
                  ? 'transform: scale(1.1)'
                  : 'transform: scale(1)' && $vuetify.theme.dark
                  ? 'box-shadow: 20px 10px 20px 0px #1976d2;'
                  : 'box-shadow: 20px 10px 20px 0px #000000;'
              "
              outlined
              shaped
              data-tilt
              @mouseover="hover[index] = true"
              @mouseleave="hover[index] = false"
            >
              <v-avatar
                size="80"
                class="display-1 font-weight-bold primary--text mb-5 justify-content-center align-items-center text-center"
                style="opacity: 1.15"
              >
                {{ card.callout }}</v-avatar
              >
              <div class="title text-uppercase pb-2" v-text="card.title"></div>
            </v-sheet>
          </NuxtLink>
          <v-row no-gutters>
            <v-col cols="12"> </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-row no-gutters> </v-row>
    </v-container>
  </section>
</template>

<script>
export default {
  data() {
    return {
      hover: {
        0: false,
        1: false,
        2: false,
      },
      pages: [
        '/reflectieverslagen/innovatieroute',
        '/reflectieverslagen/programmeerwedstrijd',
        '/reflectieverslagen/studybuddy',
      ],
      cards: [
        {
          title: 'Innovatieroute UI/UX',
          callout: '01',
        },
        {
          title: 'Vlaamse Programmeerwedstrijd 2021',
          callout: '02',
        },
        {
          title: 'Study Buddy (IT Essentials)',
          callout: '03',
        },
      ],
    }
  },
}
</script>
