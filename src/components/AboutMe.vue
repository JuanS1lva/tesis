<template>
  <section
    id="about"
    class="overflow-hidden"
  >
    <v-row
      class="white"
      no-gutters
    >
      <v-col
        class="pa-5"
        cols="12"
        md="6"
      >
        <base-bubble-1 style="transform: translate(5%, -5%)" />

        <base-heading class="info--text">
          Sobre nosotros <br>
        </base-heading>

        <base-subheading class="info--text">
          Pensamos en estas habilidades y herramientas que nos agregan valor:
        </base-subheading>

        <base-text class="mb-5">
          - Búsqueda sistemática de literatura. <br>
          - Manejo de bases de datos científicas y académicas. <br>
          - Utilización de administradores de fuentes (Ednote, Mendeley, Zotero... ). <br>
          - Experiencia en paquetes de análisis estadístico y cualitativo.<br>
          - Adaptación de la investigación a la guías de autor de la revista seleccionada.<br>
          - Expertos en diferentes áreas del conocimiento.<br>
          - Experiencia en la gestión y administración de proyectos.<br>
        </base-text>

        <!-- <v-alert
          outlined
          color="info"
        >
          <v-row
            v-for="(skill, i) in skills"
            :key="i"
            style="color: #69A1BB;"
          >
            <v-col
              class="text-uppercase"
              cols="6"
              v-text="skill.name"
            />

            <v-col
              class="text-right"
              cols="6"
              v-text="`${skill.value}%`"
            />

            <v-progress-linear
              :value="skill.value"
              color="info"
              height="8"
            />
          </v-row>
        </v-alert> -->
      </v-col>

      <v-col
        class="hidden-sm-and-down"
        md="6"
      >
        <v-img
          :src="require('@/assets/aboutme.png')"
          height="100%"
        />
      </v-col>
    </v-row>
  </section>
</template>

<script>
  export default {
    data: () => ({
      skills: [
        {
          name: 'Web Design',
          value: 100,
        },
        {
          name: 'Web Development',
          value: 75,
        },
        {
          name: 'Web Support',
          value: 90,
        },
      ],
    }),
  }
</script>
