<template>
  <v-container>
    <v-layout justify-center >
      <v-flex
        xs-12
        class="mb-6"
      >
        <h1 class="text-center"> H.J. de Vriesstraat 10</h1>
      </v-flex>
    </v-layout>
    <v-layout
      row
      justify-center
      align-center
    >
      <v-flex
        xs9
        class="mb-8"
      >
        <HomeCarousel />
      </v-flex>

    </v-layout>
    <v-layout align-center justify-center>
      <v-flex
        xs-4
        class="mb-6"
      >
        <h2 class="text-center  mb-6">Omschrijving</h2>
        <p class="text-center">Aan de H.J. de Vriesstraat no. 10/hoek Hoekstrastraat te Rainville, Paramaribo-Noord is te huur een unit groot 52m2. De locatie is bijzonder gunstig gelegen tussen de Anton Dragtenweg (op loopafstand van het Marriott Hotel) en de drukke Wilhelminastraat met verschillende voorzieningen zoals de Pizza hut, grote (banket)bakker, supermarkten, politie.</p>
      </v-flex>
    </v-layout>
    <v-layout justify-center>
      <v-flex
        xs-12
        class="mb-6"
      >
        <h2 class="text-center mb-6">Voorzieningen</h2>
        <div>
          <p class="text-center">
            <strong>
              De ruimte is voorzien van:
            </strong>
          </p>
          <ul align-center class="text-center">
            <li>Aparte elektriciteitsmeter </li>
            <li>Koud- en warmwater</li>
            <li>Keuken</li>
            <li>Airco’s</li>
            <li>Dievenijzer</li>
            <li>Alarm</li>
            <li>Telefoonaansluiting</li>
            <li>Camerabewaking</li>
            <li>Ruime Parkeergelegenheid</li>
            <li>Algehele brandverzekering</li>
          </ul>
          <p class="text-center">
            De voorwaarden voor huur worden vastgelegd in een huurcontract.
            Eén unit is sinds enige tijd verhuurd aan een Nederlands internationaal bedrijf.
          </p>
        </div>
      </v-flex>
    </v-layout>
    <v-layout justify-center>
      <v-flex
        xs-12
      >
        <h2 class="text-center mb-6">Contact</h2>
        <p class="text-center">
          Voor meer informatie:


        </p>
        <ul class="text-center">
          <li>Philomena Bijlhout</li>
          <li>Mobile Phone Suriname: +597 8735 733</li>
          <li>Nederland: +31 655598455</li>
          <li>philomenabijlhout@hotmail.com</li>
        </ul>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import HomeCarousel from '~/components/HomeCarousel.vue'

export default {
  components: {
    HomeCarousel
  }
}
</script>
