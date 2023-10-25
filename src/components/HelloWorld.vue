<template>
  <div class="mt-3 d-flex justify-between">
    <v-container class="ml-4 bg-green-darken-4 elevation-24" :class="smAndDown ? 'h-1 w-0 pl-0 pr-0 ml-10' : 'w-50'">
      <v-img src="/intro.png" cover height="400" width="800"></v-img>
    </v-container>

    <v-container class="bg-green-darken-4 mr-4 elevation-24" :class="smAndDown ? 'mr-10 mb-3' : ''">
      <h1 class="font mr-16 mt-5">ENCOMENDE AGORA<p></p>SEU MOLHO PESTO</h1>
      <h3 class="mt-5 text-light-green-lighten-4" :class="smAndDown ? 'mt-6 ml-2' : ''">Pesto é um molho italiano,
        originário
        de Gênova, na Ligúria, norte
        da Itália.<p></p> É composto tradicionalmente de folhas de manjericão <span class="text-white">(opcional)</span>
        moídas com pinhões, alho,
        sal e queijo parmesão ralado, misturados com azeite extra virgem e temperado com pimenta <span
          class="text-white">(opcional)</span> .</h3>


      <div>
        <v-dialog width="500">
          <template v-slot:activator="{ props }">
            <v-btn class="mt-10 text-green-darken-4 elevation-24" v-bind="props"
              :class="smAndDown ? 'w-75 ml-8 text-h6' : ''">
              <h5>CULINÁRIA</h5>
            </v-btn>
          </template>

          <template v-slot:default="{ isActive }">
            <v-card title="Culinária com Molho Pesto">
              <v-card-text>
                O molho pesto é uma deliciosa preparação culinária de origem italiana, conhecida pelo seu sabor fresco e
                aromático. Este molho versátil pode ser usado de várias maneiras na cozinha, acrescentando um toque
                especial a diversos pratos. É frequentemente utilizado como molho para massas, como espaguete, penne, ou
                linguine. Basta cozinhar a massa de sua escolha e misturá-la com o pesto. Pode adicionar legumes
                grelhados, frango, ou camarão para uma refeição completa e saborosa.
                O pesto também pode ser diluído com azeite de oliva e vinagre balsâmico para criar um molho de salada
                delicioso
                e aromático.

              </v-card-text>

              <v-card-actions>
                <v-spacer></v-spacer>
                <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
              </v-card-actions>
            </v-card>
          </template>
        </v-dialog>

        <div class="d-flex justify-space-between align-center">
          <v-dialog width="500">
            <template v-slot:activator="{ props }">
              <v-btn class="mt-2 text-white elevation-24 bg-green-darken-4" v-bind="props"
                :class="smAndDown ? 'w-75 ml-8 text-h6' : ''">
                <h5>BENEFICIOS</h5>
              </v-btn>
            </template>

            <template v-slot:default="{ isActive }">
              <v-card title="Beneficios do Pesto">
                <v-card-text>
                  O molho pesto se destaca por trazer diversos benefícios à saúde. Por
                  exemplo: como ele contém vitamina C, se torna um aliado na prevenção e no combate de gripes e
                  resfriados.
                  Também é importante nos cuidados com a parte cardíaca e ocular, tendo em vista que possui antioxidantes
                  e
                  nutrientes como magnésio e vitamina A. Os antioxidantes são ainda importantes para a prevenção do
                  câncer.
                  Os antioxidantes envolvidos na composição do molho pesto são ainda fundamentais para aquelas pessoas que
                  praticam exercícios físicos, sejam elas atletas de alta performance ou praticantes amadores. Isso porque
                  eles ajudam a combater os radicais livres, que são estruturas ligadas ao processo de respiração (muito
                  exigido no exercício) que levam ao envelhecimento celular precoce. Ou seja, o molho pesto pode ainda
                  melhorar a qualidade do seu treino.
                </v-card-text>

                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                </v-card-actions>
              </v-card>
            </template>
          </v-dialog>
        </div>
      </div>
    </v-container>
  </div>

  <v-container class="borda border-solid bg-green-darken-4" :class="smAndDown ? 'pl-10 pr-10' : ''" >
    <div class="d-flex align-center justify-center mt-16">
      <v-card class="borda1 pl-5 pr-5 bg-white border-solid">
        <h1 class="font text-green-darken-4">MOLHOS PESTOS</h1>
      </v-card>
    </div>


    <v-container class="d-flex justify-space-between mt-15">
      <v-card class="elevation-24" width="200" :class="smAndDown ? 'w-0' : ''">
        <v-img src="/pestorucula.png" height="200px" cover></v-img>

        <v-card-title>
          Rúcula
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 ml-2 elevation-24" :class="smAndDown ? 'w-75' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 mr-1' : ''">
        <v-img src="/pestomanjericao.jpg" height="200px" cover></v-img>

        <v-card-title>
          Manjericão
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 ml-1' : ''">
        <v-img src="/pestosalsa.jpg" height="200px" cover></v-img>

        <v-card-title>
          Salsa
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 mr-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-0' : ''">
        <v-img src="/pestoespinafre.png" height="200px" cover></v-img>

        <v-card-title>
          Espinafre
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 mr-2 ml-2">ENCOMENDAR</v-btn>
      </v-card>
    </v-container>

    <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 mr-1' : 'w-0'">
        <v-img src="/pestorucula.png" height="200px" cover></v-img>

        <v-card-title>
          Rúcula
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
        <v-img src="/pestoespinafre.png" height="200px" cover></v-img>

        <v-card-title>
          Espinafre
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 mr-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

    </v-container>


    <v-container class="d-flex justify-space-between">
      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-0' : ''">
        <v-img src="/pestotomate.png" height="200px" cover></v-img>

        <v-card-title>
          Tomate
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 ml-2">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 mr-1' : ''">
        <v-img src="/pestomanjeroxo.png" height="200px" cover></v-img>

        <v-card-title>
          Manje. Roxo
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 ml-1' : ''">
        <v-img src="/pestohortela.png" height="200px" cover></v-img>

        <v-card-title>
          Hortelã
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 mr-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-0' : ''">
        <v-img src="/pestocoentro.png" height="200px" cover></v-img>

        <v-card-title>
          Coentro
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 mr-2 ml-2">ENCOMENDAR</v-btn>
      </v-card>
    </v-container>

    <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 mr-1' : 'w-0'">
        <v-img src="/pestotomate.png" height="200px" cover></v-img>

        <v-card-title>
          Tomate
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>

      <v-card width="200" class="elevation-24" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
        <v-img src="/pestocoentro.png" height="200px" cover></v-img>

        <v-card-title>
          Coentro
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 24,90</h2>
        </v-card-subtitle>

        <v-btn class="bg-green-darken-4 mt-4 mb-2 mr-2 ml-2" :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
      </v-card>
    </v-container>
  </v-container>
</template>
 
<style scoped>
.borda {
  border-color: white;
  border-width: 10px;
  border-top-width: 0px;
  border-bottom: 0px;
}

.borda1 {
  border-color: white;
  border-width: 2px;
}

.font {
  font-family: 'Playfair Display', serif;
}

.font1 {
  font-family: 'Delicious Handrawn', cursive;
}
</style>


<script setup>
import { useDisplay } from 'vuetify';

const { smAndDown } = useDisplay()
</script>
