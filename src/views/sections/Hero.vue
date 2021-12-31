<template>
  <section id="hero">
    <v-img
      :min-height="minHeight"
      :src="require('@/assets/light.jpg')"
      class="white--text"
      gradient="to bottom, rgba(20, 20, 20, .1), rgba(0,0,0,.1)"
    >
      <v-container class="px-2 py-0">
        <v-responsive
          class="d-flex align-center mx-auto"
          height="50%"
          max-width="800"
          width="90%"
        >
        <br/><br/><br/>
        <v-card class="rounded-xl" color="#0000009D">
          <br/><br/>
          <v-row class="mx-6" align="center">
            <base-subheading
            size="text-h5"
            weight="regular"
            title="Juracar, prontos para atender quando você mais precisa!"/>
            <base-body >
              <p class="text-white">Realizamos vários serviços em seu carro. Estamos sempre prontos em atender nossos clientes.</p>
              <p class="text-white">Socorro -  Borracharia em domicílio das 07h às 22h.</p> 
              <p class="text-white">Trabalhamos com diversos serviços: mecânica em geral, borracharia, auto elétrica, balanceamento, baterias, lampadas, pneus novos e usados, vulcanização de pneus cortados.</p>
              <p class="text-white">Cuide de seu carro. Sua segurança e da sua família sempre em dia! </p>
              <p class="text-white">Conte conosco, </p>
              <p class="text-white">Equipe Juracar </p>
           </base-body>
          </v-row>
        </v-card>
        <br/><br/><br/><br/>
        </v-responsive>
      </v-container>
    </v-img>
  </section>
</template>

<script>
  export default {
    name: 'SectionHero',

    provide: {
      theme: { isDark: true },
    },

    computed: {
      minHeight () {
        const height = this.$vuetify.breakpoint.mdAndUp ? '50vh' : '25vh'

        return `calc(${height} - ${this.$vuetify.application.top}px)`
      },
    },
  }
</script>
<style type="text/css">
  rounded-card{
      border-radius:60;
  }
  p{
      color:white;
  }

</style>
