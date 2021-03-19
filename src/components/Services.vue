<template>
  <section
    id="services"
    class="overflow-hidden"
  >
    <v-col
      class="text-center pa-5"
    >
      <v-row
        class="fill-height"
        align="center"
        justify="center"
      >
        <v-col cols="12">
          <base-bubble-2
            style="transform: translateX(55%)"
          />
          <base-heading class="info--text">
            Servicios
          </base-heading>

          <base-text class="mb-5">
            Proveemos una amplia gama de servicios para ayudar a nuestro clientes a construir, implementar y publicar sus investigaciones en diferentes áreas del conocimiento.
          </base-text>
        </v-col>

        <v-col
          v-for="(service, i) in services"
          :key="i"
          class="text-center mb-3"
          sm="12"
          md="6"
          lg="4"
        >
          <v-avatar
            class="elevation-6 mb-2"
            color="#D7C9AA"
            size="64"
            tile
          >
            <v-icon
              dark
              size="52"
              v-text="service.icon"
            />
          </v-avatar>

          <base-text>
            <div
              class="mb-2 text-h6"
              v-text="service.name"
            />
            <div v-html="service.blurb" />
          </base-text>
        </v-col>
      </v-row>
    </v-col>
  </section>
</template>

<script>
  export default {
    name: 'Services',

    data: () => ({
      services: [
        {
          name: 'Trabajos De Grado',
          icon: 'mdi-book-outline',
          blurb: 'Construcción de monografias, trabajos de grado y tesis para  educación superior (pregrado, especialización y maestría) en  Ciencias de la Educación, Ciencias de la Salud, Ciencias Sociales y Humanas, Economía, Administración, Contaduría y afines, Ingeniería, Arquitectura, Urbanismo y afines. ',
        },
        {
          name: 'Articulos',
          icon: 'mdi-file-document-outline',
          blurb: 'Construcción de articulos originales, revisiones de la literatura, estudio de caso, revisión sistemática y metanálisis, búsqueda del journal para publicación y adaptación a las guias de autor exigidas.',
        },
        {
          name: 'Protocolos De Investigación',
          icon: 'mdi-card-search-outline',
          blurb: 'Creación de la propuesta de investigación, especificando objetivos, metodología de investigación y cespecificaciones para la implementación de un experimento científico.',
        },
        {
          name: 'Protocolo De Manejo Clínico',
          icon: 'mdi-medical-bag',
          blurb: 'En el ambito clinico, la cosntruccion e implementacion de protocolos de trabajo encaminados a la mediciana basada en la evidencia, con el fin de crear algoritmos de trabajo aplicables a los contextos academicos.',
        },
        {
          name: 'Revisión De Estilo, Norma Y Citación Bibliográfica',
          icon: 'mdi-file-certificate-outline',
          blurb: 'Una modalidad importate de trabajo para R & G, se basa en el trabajo activo de la aplicacion de normas y esquemas bibliograficos solicitados. Por lo cua lR & G por medio de gestores bibliograficos, garantiza la aplicacion de dichas normas de trabajo segun corresponda en cada activdad academica.',
        },
        {
          name: 'Análisis De Datos',
          icon: 'mdi-database',
          blurb: 'Análisis de datos . Diseño y creación de bases de datos, análisis estadístico y explotación de bases de datos haciendo uso de paquetes estadisticos y software de indagación cualitativa; elaboración informe de resultados.',
        },
        {
          name: 'Presentacion Para Ponencias',
          icon: 'mdi-account-group-outline',
          blurb: 'R & G, esta capacitado para realizar las revisiones tematicas desde la perspectiva profesional, para la creacion de ponencia y/o poster, de igual forma las capacitaciones y explicaciones por parte de los expertos.',
        },
        {
          name: 'Traducciones',
          icon: 'mdi-translate',
          blurb: 'En Consultorias de Investigación contamos con profesionales certificados en el área de traducción, con altos estandares de confiabilidad y calidad.',
        },
        {
          name: 'Asesoría En Investigación',
          icon: 'mdi-selection-search',
          blurb: 'Orientación para el desarrollo de trabajos y proyectos de investigación en las diferentes áreas del conocimiento.',
        },
      ],
    }),
  }
</script>
