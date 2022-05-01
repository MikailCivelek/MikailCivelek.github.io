<template>
  <section class="py-16" :class="$vuetify.theme.dark ? 'black' : ' white'">
    <v-container>
      <v-row>
        <v-col class="text-center">
          <h2 class="text-h4 text-md-h3 text-center font-weight-black">
            Activiteiten
          </h2>
          <br />
          <div
            class="text-h5 text-md-h4 text-center font-weight-black py-3 mb-10"
          >
            Verplichte activiteiten
          </div>
          <p
            class="text-md-h5 text-center font-weight-black py-3 mb-10 text-primary"
          >
            Seminaries
          </p>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(card, index) in cards"
          :key="index"
          cols="12"
          sm="4"
          class="text-center d-flex flex-column"
        >
          <v-sheet
            class="py-12 px-6 m-3 justify-center d-flex flex-column"
            style="margin: 0 auto; min-height: 500px; align-items: center"
            :style="
              $vuetify.theme.dark
                ? 'box-shadow: 20px 10px 20px 0px #1976d2;'
                : 'box-shadow: 20px 10px 20px 0px #000000;'
            "
            outlined
            shaped
            data-tilt
          >
            <v-avatar
              size="80"
              class="display-1 font-weight-bold primary--text mb-5 justify-content-center align-items-center text-center"
              style="opacity: 1.15"
            >
              {{ card.callout }}</v-avatar
            >

            <div class="title text-uppercase pb-2" v-text="card.title"></div>

            <p style="height: 200px" v-text="card.text"></p>
            <p>{{ card.datum }}, {{ card.duur }}</p>
            <p v-text="card.locatie"></p>
          </v-sheet>

          <v-row no-gutters>
            <v-col cols="12"> </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-row no-gutters> </v-row>
      <v-row>
        <v-col class="text-center">
          <p
            class="text-md-h5 text-center font-weight-black py-3 mb-10 text-primary"
          >
            Andere activiteiten
          </p>
        </v-col>
      </v-row>

      <v-row>
        <v-col
          v-for="(other, index) in others"
          :key="index"
          cols="12"
          sm="4"
          class="text-center d-flex flex-column"
        >
          <v-sheet
            class="py-12 px-6 m-3 justify-center d-flex flex-column"
            style="margin: 0 auto; min-height: 500px; align-items: center"
            outlined
            shaped
            :style="
              $vuetify.theme.dark
                ? 'box-shadow: 20px 10px 20px 0px #1976d2;'
                : 'box-shadow: 20px 10px 20px 0px #000000;'
            "
            data-tilt
          >
            <v-avatar
              size="80"
              class="display-1 font-weight-bold primary--text mb-5 justify-content-center align-items-center text-center"
              style="opacity: 1.15"
            >
              {{ other.callout }}</v-avatar
            >

            <div class="title text-uppercase pb-2" v-text="other.title"></div>

            <p style="height: 200px" v-text="other.text"></p>
            <p>{{ other.datum }}, {{ other.duur }}</p>
            <p v-text="other.locatie"></p>
          </v-sheet>

          <v-row no-gutters>
            <v-col cols="12"> </v-col>
          </v-row>
        </v-col>
      </v-row>
      <v-row no-gutters> </v-row>

      <v-row>
        <v-col class="text-center">
          <div
            class="text-h5 text-md-h4 text-center font-weight-black py-3 mb-10"
          >
            Extra activiteiten
          </div>
        </v-col>
      </v-row>
      <v-row>
        <v-col
          v-for="(extra, index) in extras"
          :key="index"
          cols="12"
          sm="4"
          class="text-center d-flex flex-column"
        >
          <v-sheet
            class="py-12 px-6 m-3 justify-center d-flex flex-column"
            style="margin: 0 auto; min-height: 500px; align-items: center"
            outlined
            shaped
            :style="
              $vuetify.theme.dark
                ? 'box-shadow: 20px 10px 20px 0px #1976d2;'
                : 'box-shadow: 20px 10px 20px 0px #000000;'
            "
            data-tilt
          >
            <v-avatar
              size="80"
              class="display-1 font-weight-bold primary--text mb-5 justify-content-center align-items-center text-center"
              style="opacity: 1.15"
            >
              {{ extra.callout }}</v-avatar
            >

            <div class="title text-uppercase pb-2" v-text="extra.title"></div>

            <p style="height: 200px" v-text="extra.text"></p>
            <p>{{ extra.datum }}, {{ extra.duur }}</p>
            <p v-text="extra.locatie"></p>
          </v-sheet>

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
      cards: [
        {
          title: 'Cap Gemini (Unit Testing)',
          text: 'In deze seminarie heb ik meer geleerd over Unit Testing en de best practices hiervan. Daarnaast hebben we zelf ook een paar Unit-testen kunnen schrijven en hierop werd ook feedback gegeven hoe we het beter konden doen volgens de best practices. Er was ook een kleine introductie in test driven development. Ten slotte hebben we ook de meest voorkomende fouten besproken en hoe we deze kunnen vermijden.',
          datum: '18 februari 2020',
          locatie: 'Hogeschool PXL',
          duur: '4 uur',
          callout: '01',
        },
        {
          title: 'Wheelhouse (JAMstack)',
          text: 'In deze seminarie wordt er niet over een technologie gepraat, maar over een manier van werken, namelijk JAMstack (Javascript APIs Markup-stack). De Jamstack-architectuur heeft vele voordelen, of het nu gaat over een grote e-commercesite, SaaS-toepassing of persoonlijke blog. Daarnaast is er gesproken hoe je aan JAMstack begint en is er een demonstratie gegeven van een website met deze werkwijze.',
          datum: '23 maart 2021',
          locatie: 'Microsoft Teams Online',
          duur: '3 uur',
          callout: '02',
        },
        {
          title: ' Solita (iPaaS) ',
          text: 'In deze seminarie werd er uitgelegd wat iPaaS precies is en hoe het kan helpen om complexe bedrijfsintegraties efficiënt te ontwikkelen. Er is kennisgemaakt met de concepten van iPaaS, API management, events, messaging, enz. Vervolgens hebben we ook oefeningen kunnen maken om een aantal realtime implementaties te zien op Azure en SnapLogic.',
          datum: '30 maart 2021',
          locatie: 'Microsoft Teams Online',
          duur: '3 uur',
          callout: '03',
        },
        {
          title: 'Datasense (Snowflake)',
          text: 'In deze seminarie wordt er uitgelegd over Snowflake, een datawarehouse-systeem dat zeer snel gegevens kan verwerken. Vervolgens vertelt Niels over de uitdagingen van datawarehouse-projecten. Daarnaast is er meer diepgang over wat Snowflake precies is en de voordelen hiervan. Na deze infosessie hebben de studenten de kans gekregen om zelf een aantal oefeningen te maken op het platform.',
          datum: '10 november 2021',
          locatie: 'Hogeschool PXL',
          duur: '3 uur',
          callout: '04',
        },
        {
          title: 'Accenture (Cloudhosting)',
          text: 'In deze seminarie wordt er uitgelegd over applicaties gehost op de cloud en de voordelen hiervan. Ook het hele proces van bedrijfsdoelstellingen identificeren tot en met cloud als een leveringsplatform is uitgelegd. Daarnaast is er ook basiskennis gedeeld van docker-images om de studenten genoeg uitleg te geven zodat ze kunnen volgen.',
          datum: '1 december 2021',
          locatie: 'Microsoft Teams Online',
          duur: '3 uur',
          callout: '05',
        },
        {
          title: 'Eurofins (Docker)',
          text: 'In deze seminarie hebben studenten geleerd wat Docker precies is en hoe het werkt. Vervolgens heeft Martijn uitgelegd hoe Docker de meest voorkomende problemen in applicatieontwikkeling oplost. Daarnaast heeft hij ook de verschillen en gelijkenissen aangehaald tegenover virtual machines. Hierna hebben we ook de kans gekregen om een Docker-container op te zetten en hiermee te experimenteren.',
          datum: '8 december 2021',
          locatie: 'Microsoft Teams Online',
          duur: '3 uur',
          callout: '06',
        },
        {
          title: 'Konsolidate (Solid)',
          text: 'In deze seminarie vertelt Christophe over Solid. Specifiek, praat hij over de problemen die Solid oplost en hoe het wordt geïntegreerd in de hedendaagse technologieën. Vervolgens geeft hij nog enkele use-cases hiervan om de studenten een beter inzicht te geven. Ten slotte hebben de studenten de kans gekregen om zelf een oefening te maken en werd deze ook samen verbeterd.',
          datum: '15 december 2021',
          locatie: 'Microsoft Teams Online',
          duur: '3 uur',
          callout: '07',
        },
        {
          title: 'Bewire (Spring Batch)',
          text: 'In deze seminarie wordt Spring Batch voorgesteld. Dit is een lichtgewicht, uitgebreid batch framework ontworpen om de ontwikkeling van robuuste batch applicaties mogelijk te maken die van essentieel belang zijn voor de dagelijkse werking van bedrijfssystemen.',
          datum: '21 april 2022',
          locatie: 'Youtube Live',
          duur: '3 uur',
          callout: '08',
        },
        {
          title: 'Refleqt (Cypress)',
          text: 'In deze seminarie hebben we informatie gekregen over Continious Devolopment en vervolgens over Cypress. Dit is een  frontend test tool, gebouwd voor het moderne web. Het richt zich op de pijnpunten waar ontwikkelaars of QA engineers tegenaan lopen tijdens het testen van een applicatie.',
          datum: '26 april 2022',
          locatie: 'Hogeschool PXL',
          duur: '3 uur',
          callout: '09',
        },
      ],
      others: [
        {
          title: 'Innovatieroute UI/UX',
          text: 'In deze innovatieroute hebben studenten informatie gekregen over UI en UX. Vervolgens hebben studenten de kans gekregen deze leerstof toe te passen met zelf mock-ups te maken. Hierna hebben studenten hun zelfgemaakte applicaties met hun ideeën kunnen presenteren en hebben ze hierop ook feedback gekregen.',
          datum: '30 september 2021 t.e.m. 14 oktober 2021',
          locatie: 'Hogeschool PXL',
          duur: 'elke donderdag 8 uur lang',
          callout: '01',
        },
        {
          title: 'POP-Sessie: My Teeam and I',
          text: 'In deze interactieve POP-sessie hebben we de kans gekregen om samen met andere studenten enkele activiteiten uit te voeren. De teams waren de originele teams van het IT-project en de doel van deze sessie was om de teambuilding te versterken. Hierdoor leerden we elkaar beter kennen en had het een positieve invloed op ons samenwerking. Ook kwam elkaars zwakke en sterke punten aanbod.',
          datum: '26 april 2022',
          locatie: 'Hogeschool PXL',
          duur: '3 uur',
          callout: '02',
        },
        {
          title: 'POP-Sessie: Brein aan het werk, niet storen !',
          text: 'In deze POP-sessie hebben we meer inzicht gekregen over onze gewoontes en routines. We hebben alles op tafel gelegd en hun ingedeeld in vier categorieën namelijk: belangrijk, niet belangrijk, dringend en niet dringend.',
          datum: '3 maart 2020',
          locatie: 'Hogeschool PXL',
          duur: '3 uur',
          callout: '03',
        },
        {
          title: 'POP-Sessie: (Veer)krachtige teams',
          text: 'In deze POP-sessie hebben we als een team gewerkt om enkele activiteiten uit te voeren. Deze dienden om onze teamgenoten te leren vertrouwen en met constructieve feedback om te gaan zodat we kunnen groeien als team en individueel. Daarnaast leerden we ook wat het betekent om een teamspeler te zijn en wat een goed team is.',
          datum: '3 maart 2020',
          locatie: 'Hogeschool PXL',
          duur: '3 uur',
          callout: '04',
        },
        {
          title: 'Projectweek',
          text: 'Tijdens deze week heb ik verschillende seminaries gevolgd en verschillende teambuilding activiteiten uitgevoerd. Studenten hebben ook hun kernkwaliteiten en valkuilen besproken. Hiernaast hebben studenten ook het Thalento-test afgelegd en werd er informatie gegeven over hoe studenten groepsprojecten goed kunnen aanpakken.',
          datum: '10 februari 2020 t.e.m. 14 februari 2020',
          locatie: 'Hogeschool PXL',
          duur: 'elke dag hele week',
          callout: '05',
        },
        {
          title: 'Hackathon: PXL-Research',
          text: 'Tijdens deze hackathon, georganiseerd door Hogeschool PXL, hebben we de kans gekregen om te werken met Unity. Hierin hebben studenten verschillende games gemaakt voor mensen met een beperking. Het was een leerrijke en interessante ervaring die studenten zeker aansprak.',
          datum: '10 februari 2020 t.e.m. 14 februari 2020',
          locatie: 'Hogeschool PXL',
          duur: 'twee keer acht uur',
          callout: '06',
        },
      ],
      extras: [
        {
          title: 'Hackathon: Hack The Future',
          text: 'In deze hackathon hebben een aantal groepen gewerkt met PowerApps. Het onderwerp van de hackathon was een onderzoek uitgevoerd door een rechercheur. De rechercheur zou dan de applicatie kunnen raadplegen om alle informatie in te voeren, updaten, bekijken of verwijderen.',
          datum: '2 december 2021',
          locatie: 'Online Hackathon',
          duur: '10 uur',
          callout: '01',
        },
        {
          title: 'Study Buddy (IT Essentials)',
          text: 'Ik heb twee studenten bijles gegeven over het vak IT Essentials. Dit was leerrijk voor hun maar ook voor mij omdat ik mee geleerd heb als begeleider en mijn vaardigheden in Python heb herhaald.',
          datum: 'oktober 2021 – november 2021',
          locatie: 'Hogeschool PXL, Corda Campus, Microsoft Teams Online',
          duur: '20 uur',
          callout: '02',
        },
        {
          title: 'Vlaamse programmeerwedstrijd 2021',
          text: 'Meer dan tien groepen van studenten namen deel aan het jaarlijkse wedstrijd. Vervolgens had mijn team de voorkeur om de vijf oefeningen te maken in Python. Het was een interessante en intensieve uitdaging waarvan het de deelname waard was.',
          datum: '2 december 2021',
          locatie: 'Online wedstrijd',
          duur: '10 uur',
          callout: '03',
        },
      ],
    }
  },
}
</script>
