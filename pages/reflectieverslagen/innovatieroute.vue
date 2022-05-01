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
      Innovatieroute UI/UX
    </h2>
    <br />
    <div class="row">
      <div class="col-lg-10 m-auto">
        <p
          class="justify-content-center max-auto mx-auto"
          style="text-align: justify"
        >
          De innovatieroute UI/UX werd gehouden tussen 30 september en 20
          oktober op donder- en vrijdagen en ging door op de B-blok van
          Hogeschool PXL. De innovatieroute was een samenstellingen van drie
          verschillende seminaries die gegeven werden door twee bedrijven,
          namelijk Appwise en Appfoundry/Humix. <br /><br />
          De eerste dag was meer informatief en was er uitleg gegeven door
          Appwise. Dit bedrijf zet zich sterk in en begrijpt ook de aspecten van
          UI/UX. Ze werken dagelijks aan projecten die uitgewerkt worden met
          respect naar de gebruiksvriendelijkheid en ervaring. Hierdoor heeft
          dit bedrijf ons geïnformeerd waarom ze het zo belangrijk vinden om
          aandacht te besteden aan het ontwerp van de applicatie vooraleer ook
          enige code geschreven is. Ze werken samen met de klant en houden ze
          ook dichtbij. Hiermee bedoel ik dat de klanten begeleid worden door
          het volledige ontwikkelingsproces van de applicatie. Ze hebben
          hierdoor iteratief feedback en zijn zo een ervaren bedrijf geworden
          die de noden van de klant snel kan begrijpen.<br /><br />
          Vervolgens heeft Appwise ons uitgelegd wat er allemaal aanbod komt in
          het maken van een ontwerp. Als eerste stap is er de customer journey
          matrix. Dit houdt in dat alle uitdagingen van de gebruiker worden
          weergegeven wanneer de gebruiker een bepaalde actie wilt voltooien. De
          eerste kolom toont alle vragen die beantwoord zullen worden, terwijl
          de eerste rij alle processen opsomt die de gebruiker doorloopt. Alle
          moeilijkheden en uitdagingen voor de gebruiker wordt achteraf getoond
          wanneer deze proces is voltooid. Hierna krijg je een diagram dat het
          resultaat weergeeft met alle activiteiten dat de gebruiker kan
          doorlopen. Vervolgens konden wij zelf aan de slag gaan om de mobiele
          applicatie van Tinder te analyseren. De hoofdvraag was wat we zouden
          verbeteren aan Tinder. Hiervoor werden studenten ingedeeld in groepen
          van vier à vijf personen om deze vraag te beantwoorden. Tijdens deze
          taak kwam mijn groep op het idee om een date te kunnen plannen met je
          match in de applicatie zelf. Dit zorgt ervoor dat de gebruiker niet
          snel geneigd is om de applicatie te sluiten om ideeën voor dates op te
          zoeken en deze tevoorschijn krijgt in de applicatie. Hierna heeft elk
          team een korte presentatie gegeven over hun ideeën en hebben ze hierop
          feedback gekregen.<br /><br />
          De volgende twee dagen had Appfoundry/Humix ons een mobiele applicatie
          laten ontwerpen met als concept om een probleem binnen de school op te
          lossen. Voor deze workshop werden studenten ingedeeld in groepen van
          vier à vijf studenten om zo ons beter te kunnen begeleiden en teamwerk
          te stimuleren. Als eerste stap van de workshop, konden we een paar
          concepten uitwerken van de gebruikservaring met de gebruiker centraal.
          Tijdens deze workshop heeft mijn team gekozen om een meer indirect
          probleem aan te pakken, namelijk het slaapritme van de student.<br /><br />
          Na het kiezen van het onderwerp, kon elk team brainstormen over
          belangrijke aspecten van hun applicatie. Vervolgens heeft elk team een
          aantal suggesties opgeschreven een vorm van “post-it”-briefjes en
          stemde ze op de suggestie die hen het meest aansprak. Nadat we ons
          onderwerp hadden en het idee van de applicatie, konden we beginnen met
          de “hoe kunnen we”-vragen te beantwoorden. Daarna had elk team gezocht
          naar een oplossing voor hun probleem. Dit was een belangrijk stap om
          onze applicatie te kunnen realiseren, de doelstellingen over na te
          kunnen denken en realistisch te blijven over de verwachtingen.<br /><br />Op
          de laatste dag hadden we wireframes gemaakt van de user interface. Een
          wireframe is een blauwdruk dat weergeeft hoe de gebruiker de
          applicatie doorloopt, het is meer gefocust op de functionaliteit van
          de applicatie. Elk team heeft de kans gekregen om hun kennis toe te
          passen op de wireframes. Dit houdt in de gebruiksvriendelijkheid en
          gebruikservaring. In de gebruiksvriendelijkheid hebben we nagedacht
          over de overzichtelijkheid van de applicatie, dat alles makkelijk
          terug te vinden is en opgebouwd is met een logische structuur. De
          gebruikservaring heeft van belang dat wanneer de gebruiker een
          bepaalde actie wilt uitvoeren, het een efficiënt en simplistisch
          proces is waarvoor de gebruiker niet veel interactie zou moeten
          uitvoeren. Als laatste hadden we gebruikgemaakt van de wireframes om
          de mock-ups te ontwikkelen. Deze stap verbindt alles van onze kennis
          tot een interactieve applicatie. Hierna heeft elk team de kans
          gekregen om hun applicatie te presenteren en constructieve feedback te
          ontvangen. <br /><br />
          De innovatieroute leek me interessant vanwege het onderwerp. Ik wou me
          altijd verdiepen in UI/UX. Ook al maak ik kleine applicaties hier en
          daar, deze concepten komen altijd aanbod. Voor deze innovatieroute was
          ik meer geïnteresseerd in backend-ontwikkeling, maar mijn perspectief
          is aangepast na deze innovatieroute. Ik ken een aantal frontend
          frameworks en wat HTML, CSS en JS om deze te ondersteunen, maar niet
          over concepten van UI/UX. Hierdoor heb ik kritisch kunnen terugkijken
          naar de applicaties die ik al heb gemaakt en heb ik mijn vordering al
          meteen gemerkt. Dit laat zien dat ik nog veel te leren heb en altijd
          een betere ontwikkelaar kan worden. Daarnaast besteed ik nu meer
          aandacht aan de gebruikservaring en gebruiksvriendelijkheid wanneer ik
          een applicatie maak.<br /><br />
          Ik heb deze opdracht gekozen omdat ik hier veel heb bijgeleerd. Ik
          dacht dat mijn applicaties altijd aan de voorwaarde voldoen om te
          tellen als een gebruiksvriendelijke applicatie, maar dit was een
          oogopener dat er details waren waar ik niet naar gekeken heb. Ik zie
          UI/UX nog altijd als een sterke punt van mezelf maar vind ik dat ik
          zeker nog kan verbeteren op dit vlak. Ook is het een onderwerp dat
          toegepast wordt in mijn opleiding. Voor school maken we altijd
          verschillende programma’s, groot of klein, team of alleen, waarvoor er
          een interface is voorzien. Als het nu een simpele of complexe
          interface is, komen deze concepten altijd aanbod.<br /><br />
          Vervolgens zie ik ook het nut en belang van een concept volgens een
          stappenplan uit te werken. Je kan bepaalde conceptuele fouten vroeg
          opsporen zodat je geen werk levert dat uiteindelijk niet gebruikt kan
          worden. Dit houdt in dat je de noden van de gebruiker begrijpt, de
          oplossingen bedenkt, de concepten overzet in wireframes, na de
          functionele wireframes het concept omzet naar mock-ups en ten slotte
          een werkende applicatie maakt.Ik zal deze stappen respecteren als ik
          in de toekomst een applicatie zal maken.<br /><br />
          Ik had geen problemen met de innovatieroute of de leerstof die
          gepresenteerd werd, alles werd grondig uitgelegd en werden we goed
          begeleid door de bedrijven daarnaast is het geen nieuw onderwerp voor
          mij. Na de innovatieroute heb ik ook connecties kunnen maken met
          Appwise en Appfoundry op LinkedIn en heb deze ook gecontacteerd in
          verband met een stage. Helaas, heb ik mijn stage niet bij hun
          uitgevoerd, maar zal hun terug contacteren na mijn stage.
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
          src: '/i_1.png',
        },
        {
          src: '/i_2.png',
        },
        {
          src: '/i_3.png',
        },
        {
          src: '/i_4.png',
        },
        {
          src: '/i_5.png',
        },
      ],
      //
    }
  },
}
</script>
