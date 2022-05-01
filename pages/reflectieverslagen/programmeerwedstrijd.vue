<template>
  <section id="innovatieroute" :class="$vuetify.theme.dark ? 'black' : 'white'">
    <div class="m-auto col-lg-10">
      <v-carousel
        height="calc(70vh - 64px)"
        cycle
        show-arrows-on-hover
        hide-delimiter-background
      >
        <v-carousel-item
          v-for="(carousel, carindex) in carouselsData"
          :key="carindex"
          :src="carousel.src"
        >
        </v-carousel-item>
      </v-carousel>
    </div>

    <h2 class="text-h4 text-md-h3 text-center font-weight-black mb-8 my-8">
      Vlaamse Programmeerwedstrijd 2021
    </h2>
    <br />
    <div class="row">
      <div class="col-lg-10 m-auto">
        <p
          class="justify-content-center max-auto mx-auto"
          style="text-align: justify"
        >
          De wedstrijd werd gehouden door AP Hogeschool in samenwerking met
          verschillende andere universiteiten en hogescholen op 21 maart 2021.
          De doelstellingen van deze wedstrijd was om als snelste team de vijf
          oefeningen te voltooien binnen een bepaalde tijd. Ik heb deelgenomen
          samen met twee medestudenten genaamd Murat Bataray en Zeyd Uysal. Deze
          twee studenten studeren ook aan de Hogeschool PXL.<br /><br />
          Als voorbereiding heeft ons team een aantal oefeningen gemaakt om zo
          onze kennis van Python op te frissen. In details houdt dit in dat we
          onze functies, condities, iteraties, bibliotheken, wiskundige
          berekeningen en ook formules hebben herhaald. Daarnaast heeft elk team
          het recht om code te gebruiken die zal al hadden voorbereid. Vandaar
          ook dat dit een belangrijk proces was als je de oefeningen wou maken
          op een snelle en efficiënte manier.<br /><br />
          Dit jaar was het evenement geen klassieke Olympiade, maar een
          volledige online editie in het thema van Dungeons & Dragons. De beste
          teams winnen naast eeuwige roem ook een leuke prijs. Het programma
          begon om 12:30 met online de deuren te openen. Vervolgens konden we
          een kwartier later ons verzamelen in de lobby. Nadat deze verzameling
          voltooid was, gaf de jury een toespraak over het evenement, maar kwam
          het wedstrijdreglement ook aanbod. Na deze inlichting ging de
          wedstrijd van start van de verschillende categorieën. Mijn team
          behoorde tot de tweede categorie namelijk de professionele
          bachelorstudenten. In de wedstrijd hadden we drie uur de tijd om deze
          uitdagende oefeningen uit te werken. Na deze intensieve periode was er
          een prijsuitreiking waarna de event ook tot een succesvolle einde
          kwam.<br /><br />
          Tijdens de wedstrijd waren we toch wel verrast van onze tijdelijke
          score. Dit was omdat we altijd binnen de top vijf waren van tientallen
          teams. Dit gaf ons een boost om verder te werken en misschien in de
          top drie te belanden. Daarnaast waren de oefeningen zelf complex en de
          wedstrijd laat ook zien waarom je een team nodig zal hebben. Als je
          hier zelf aan zou werken zou dit een langdurig en complexe proces
          zijn. Als team, kan je de oefeningen opdelen in meerdere
          deeloefeningen en andere aanpakken krijgen van je teamleden, dit zorgt
          voor ideeën die snel bedacht en uitgevoerd kunnen worden. Daarnaast is
          er ook de druk van andere teams en de tijdsdruk van de wedstrijd zelf.
          Dit zorgt ervoor dat je als team snel beslissingen moet nemen. Mijn
          team heeft besloten om de team op te splitsen in twee teams. Een
          teamgenoot zou al aan een andere oefening werken terwijl ik en een
          ander teamgenoot samen aan een specifieke oefening verder werkten. Dit
          heeft ervoor gezorgd dat we sneller vordering hadden, maar
          uiteindelijk waren de oefeningen te complex om alleen aan een
          oplossing te komen en uitschrijven. Hierdoor hebben we uiteindelijk
          deze aanpak geschrapt en toch als een team verder gewerkt.<br /><br />
          Uiteindelijk hebben we toch een resultaat kunnen behalen. Hiermee
          bedoel ik dat we als vijfde zijn geëindigd en één ander PXL-team boven
          ons heeft gepresteerd. Alleen de eerste top drie kwam in aanmerking
          met de prijzen, maar was het nog steeds een leerrijke ervaring. Ook
          hebben we een mail gekregen van Arno Barzan die ons heeft
          gefeliciteerd van onze prestatie en deze wedstrijd heeft opgenomen in
          het vak I-talent. Om deze kans maximaal te benutten hebben we ook
          connecties gemaakt met het ander PXL-team op LinkedIn. Vervolgens
          hebben we ook een LinkedIn-post gemaakt van het behaalde resultaat om
          zo verder ons netwerk uit te breiden.<br /><br />
          Voor deze wedstrijd heb ik een voorbereiding gemaakt zodat we al code
          hadden aan de start van de wedstrijd. Dit was omdat het een nodige
          proces was als we een kans wouden om te winnen. In de wedstrijd zelf
          heb ik vooral aan pair-programming gedaan met mijn teamleden. Eerst
          was het moeilijker om samen te werken omdat elk hun versie van de
          oefening wou uitwerken met hun ideeën. Hierdoor hebben we wat
          vertraging opgelopen, maar dit probleem hebben we kunnen oplossen door
          ieder zijn versie van de oefening te maken en dan informatie te delen.
          Hierdoor kwamen we snel aan een werkende oplossing voor de oefening
          Overal, was het een leerrijke ervaring, niet alleen om mijn
          vaardigheden van Python te verbeteren, maar ook op persoonlijk vlak.
          Ik heb geleerd in een stressvolle omgeving kalm te blijven en samen
          als team door te pushen voor een mooie resultaat. Mijn zwakke punt was
          dat ik moeite had om mijn ideeën in code krijgen, maar mijn teamleden
          konden mij hierbij helpen. Hiernaast was mijn sterke punt dat ik
          verschillende ideeën had om de oefeningen uit te werken en kwam zo aan
          verschillende oplossingen die mijn teamleden hebben kunnen coderen.
          Ook heeft deze ervaring mij geholpen om in team te werken voor komende
          projecten voor school waarvoor teamwerk van belang is.<br /><br />
          Ik heb deze opdracht gekozen omdat ik hieruit veel heb kunnen leren in
          verschillende categorieën. Ik heb mijn vaardigheden kunnen testen
          vergeleken met andere studenten, vervolgens dat ik mezelf persoonlijk
          heb kunnen ontwikkelen. Daarnaast heb ik ook mijn netwerk kunnen
          uitbreiden voor mijn carrière in de toekomst. Dit vind ik belangrijk
          om mijn kansen in deze sector te maximaliseren
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      carouselsData: [
        {
          src: '/v_1.jpg',
        },
        {
          src: '/v_2.jpg',
        },
        {
          src: '/v_3.jpg',
        },
        {
          src: '/v_5.png',
        },
      ],
      //
    }
  },
}
</script>
