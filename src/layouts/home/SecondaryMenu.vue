<template>
  <v-menu
    v-model="menu"
    :close-on-content-click="true"
    bottom
    left
    max-width="80%"
    min-width="320"
    offset-x
    offset-y
    origin="top left"
    transition="scale-transition"
  >
    <template #activator="{ attrs, on }">
      <v-card
        id="secondary-menu"
        class="py-2 px-4"
        color="#b45e00"
        dark
        flat
        style="position: fixed; top: 100px; left: -10px; text-align: right;"
        width="180"
        v-bind="attrs"
        v-on="on"
      >
       
        Endereços
         <v-icon large >
          mdi-google-maps
        </v-icon>
      </v-card>
    </template>

    <v-card class="py-2">
      <br/>
      <base-title
        align="center"
        title="Endereços"
        space="0"
      />

      <v-card-text>
        <v-item-group
         
          class="d-flex justify-center"
        >
        </v-item-group>

        <v-divider class="my-6" />


       <div
          class="mr-4"
         
        >
          <v-icon left>
            mdi-google-maps
          </v-icon>
          <a href="https://goo.gl/maps/jSAQVLUaqGfpqBkHA" style="color:#000000 font-family: arial !important;">Rua Artur de Azevedo, 891 - Pinheiros - SP</a>
        </div>
     


         
      </v-card-text>
    </v-card>
  </v-menu>
</template>

<script>
  export default {
    name: 'HomeSettings',

    data () {
      return {
        colors: [
          this.$vuetify.theme.currentTheme.primary,
          '#9368e9',
          '#F4511E',
        ],
        menu: false,
      }
    },

    computed: {
      currentThemePrimary: {
        get () {
          return this.$vuetify.theme.currentTheme.primary
        },
        set (val) {
          const target = this.$vuetify.theme.isDark ? 'dark' : 'light'

          this.$vuetify.theme.themes[target].primary = val
        },
      },
    },
  }
</script>
