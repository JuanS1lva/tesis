<template>
  <section
    id="welcome"
    class="overflow-hidden"
  >
    <v-row no-gutters>
      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/chica_frustrada.jpg')"
          height="100vh"
        />
      </v-col>

      <v-col
        class="align-content-space-between layout wrap"
        cols="12"
        md="6"
      >
        <base-bubble-1
          style="transform: rotate(180deg) translateY(25%)"
        />

        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="12"
            md="6"
            class="py-14 ml-8"
          >
            <base-heading>¿Bloqueado en tu investigación?</base-heading>
            <base-text>
              Te ayudamos a resolver las dificultades con tu proyecto.
            </base-text>
            <base-btn
              class="mt-4"
              href="#services"
            >
              Conoce nuestros servicios
            </base-btn>
          </v-col>
        </v-row>

        <base-bubble-2
          style="transform: rotate(180deg) translate(-200px, -15%)"
        />
      </v-col>
    </v-row>
  </section>
</template>
