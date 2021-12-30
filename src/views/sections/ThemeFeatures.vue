<template>
  <base-section id="theme-features">
   <base-section-heading id="servicos" title="Serviços">
    </base-section-heading>
    
    <v-container>
      <v-row>
        <v-col
          v-for="(feature, i) in features"
          :key="i"
          cols="12"
          md="6"
        >
          <base-avatar-card
            v-bind="feature"
            align="left"
            horizontal
          >
            {{text}}
          </base-avatar-card>
        </v-col>
      </v-row>
    </v-container>
   <base-section-heading id="galeria" title="Galeria">
      <v-row justify="center">
        <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/1.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
          </v-img>
        </v-col>
        <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/2.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>

       <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/3.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>

       <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/4.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>

       <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/5.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>
      
      <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/6.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>
       <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/7.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>
       <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/8.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>
       <v-col
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="require('@/assets/9.jpg')"
            
            aspect-ratio="1"
            class="grey lighten-2"
          >
        </v-img>
       </v-col>
  
    </v-row> 
   </base-section-heading>

  </base-section>
  

</template>

<script>
  export default {
    name: 'SectionThemeFeatures',

    data: () => ({
      features: [
  
        {      
          title: 'Mecânica em geral',
          icon: 'mdi-tools',
          text:'Serviços gerais de mecânica. Traga seu carro para uma avaliação.'
        
        },
    
        {
          title: 'Borracharia',
          icon: 'mdi-tire',
          text:'Fazemos o melhor para que os pneus de seu carro estejam prontos para o dia a dia ou estrada.'
        },
          {
          title: 'Auto elétrica',
          icon: 'mdi-lightning-bolt',
          text: 'Serviços de elétrica automotiva em geral. Se percebeu algo estranho, não exite e traga para fazermos uma avaliação.'

        },
        {
          title: 'Balanceamento',
          icon: 'mdi-road-variant',
          text: 'Desconforto ao dirigir? Direção tremendo? Utilize seu carro de forma prazerosa com os pneus corretamente balanceados.'

        },
        
        {
          title: 'Baterias',
          icon: 'mdi-star',
          text: 'As melhores marcas de bateria para você não ficar parado!'

        },
        
        {
          title: 'Lampadas',
          icon: 'mdi-lightbulb',
          text: 'Lampadas automotivas em geral.'

        },

        {
          title: 'Pneus novos e usados',
          icon: 'mdi-tire',
          text: 'Venha escolher seu pneu novo ou mesmo a troca por um usado em boas condições. Passe por uma análie com nossa equipe.'

        },
        
        {
          title: 'Vulcanização de pneus',
          icon: 'mdi-fire',
          text: 'Pneu rasgado ou danificado? Não compre outro somente por isso, podemos resolver com uma vulcanização. Venha conferir!'

        },
      ],
    }),
  }
</script>

