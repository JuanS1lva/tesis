<template>
  <div>
    <v-btn
      v-for="(item, i) in items.slice(0, large ? items.length : 1)"
      :key="i"
      fab
      class="ma-2"
      color="info"
      :small="!large"
      :href="item.redir"
      target="_blank"
    >
      <v-icon
        dark
        v-text="item.icon"
      />
    </v-btn>
  </div>
</template>

<script>
  export default {
    props: {
      large: {
        type: Boolean,
        default: false,
      },
    },

    data: () => ({
      items: [
        {
          name: 'WhatsApp',
          icon: 'mdi-whatsapp',
          redir: 'https://wa.link/7lduct',
        },
        {
          name: 'Instagram',
          icon: 'mdi-instagram',
          redir: 'www.google.com',
        },
        {
          name: 'Facebook',
          icon: 'mdi-facebook',
          redir: 'www.google.com',
        },
        {
          name: 'Email',
          icon: 'mdi-email',
          redir: 'www.google.com',
        },
        {
          name: 'Phone',
          icon: 'mdi-phone',
          redir: 'www.google.com',
        },
      ],
    }),
  }
</script>
