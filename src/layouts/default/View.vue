<template>
  <v-main>
    <router-view />
  </v-main>

  <v-app>
    <v-img src="/fundo.jpg" class="background-image" cover>

      <div class="d-flex justify-between elevation-24">
        <v-container class="bg-green-darken-4 elevation-24 ml-4" :class="smAndDown ? 'mt-3 pr-0 ml-12 mb-3' : ''">
          <h1 class="font mr-16 mt-5">ENCOMENDE AGORA<p></p>SEU AZEITE SABORIZADO</h1>
          <h3 class="mt-5 text-light-green-lighten-4" :class="smAndDown ? 'mt-6 ml-2' : ''">O azeite é um ingrediente
            essencial em cozinhas de todo o mundo, tão antigo quanto a própria humanidade. <p></p>Mas ainda existem muitas
            curiosidades sobre o azeite de oliva que nem todo mundo conhece.</h3>

          <div>
            <v-dialog width="500">
              <template v-slot:activator="{ props }">
                <v-btn class="mt-10 text-green-darken-4 elevation-24" v-bind="props"
                  :class="smAndDown ? 'w-75 ml-8 text-h6' : ''">
                  <h5>CULINÁRIA</h5>
                </v-btn>
              </template>

              <template v-slot:default="{ isActive }">
                <v-card title="Culinária com Azeite">
                  <v-card-text>
                    O azeite é um ingrediente fundamental na culinária, amplamente utilizado em diversas cozinhas ao redor
                    do mundo devido ao seu sabor, versatilidade e benefícios à saúde. Sendo também um ótimo meio para
                    refogar e saltear vegetais, carnes e frutos do mar. Ele oferece uma base saborosa e evita que os
                    alimentos grudem na panela. Use azeite extra virgem para preservar o seu sabor. O azeite é um
                    componente
                    essencial em muitos molhos e vinagretes. Combine-o com vinagre, suco de
                    limão, ervas, alho e outros temperos para criar molhos saborosos para saladas, massas ou legumes
                    grelhados.
                  </v-card-text>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                  </v-card-actions>
                </v-card>
              </template>
            </v-dialog>
          </div>

          <v-dialog width="500">
            <template v-slot:activator="{ props }">
              <v-btn class="mt-2 text-white elevation-24 bg-green-darken-4" v-bind="props"
                :class="smAndDown ? 'w-75 ml-8 text-h6' : ''">
                <h5>BENEFICIOS</h5>
              </v-btn>
            </template>

            <template v-slot:default="{ isActive }">
              <v-card title="Beneficios do Azeite">
                <v-card-text>
                  O azeite de oliva também é conhecido por seus inúmeros benefícios à
                  saúde. Originário das oliveiras, ele é repleto de ácidos graxos monoinsaturados, especialmente o ácido
                  oleico, que desempenham um papel fundamental na promoção da saúde cardiovascular. Reduzindo o colesterol
                  ruim e aumentando o colesterol bom, o azeite protege o coração e reduz o risco de doenças cardíacas.
                  Além disso, o azeite de oliva é um verdadeiro escudo contra a inflamação, ajudando a combater doenças
                  crônicas. Seu alto teor de antioxidantes, incluindo a vitamina E, protege as células contra danos
                  causados
                  pelos radicais livres, retardando o envelhecimento e fortalecendo o sistema imunológico.
                </v-card-text>

                <v-card-actions>
                  <v-spacer></v-spacer>
                  <v-btn text="Fechar" @click="isActive.value = false"></v-btn>
                </v-card-actions>
              </v-card>
            </template>
          </v-dialog>
        </v-container>

        <v-container class="bg-green-darken-4 elevation-24 mr-4" :class="smAndDown ? 'h-1 w-0 pl-0 pr-0 ml-10' : 'w-50'">
          <v-img src="/fundo1.png" cover height="400" width="800"></v-img>
        </v-container>
      </div>

      <v-container class="cont1 bg-white border-solid">
        <div class="cont1 d-flex align-center justify-center mt-16">

          <v-card class="card1 pl-5 pr-5 bg-green-darken-4 border-solid">
            <h1 class="font text-white" :class="smAndDown ? 'ml-1' : ''">AZEITES</h1>
          </v-card>
        </div>
      </v-container>


      <v-container class="border-solid cont1 bg-white">

        <v-container class="d-flex justify-space-between mt-15">
          <v-card class="elevation-24 bg-green-darken-4" width="200" :class="smAndDown ? 'w-0' : ''">
            <v-img src="azeitealecrim.jpg" height="200px" cover></v-img>

            <v-card-title>
              Alecrim
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white-4 mt-4 mb-2 ml-2 elevation-24 text-green-darken-4"
              :class="smAndDown ? 'w-75' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 mr-1' : ''">
            <v-img src="azeitegengibre.jpg" height="200px" cover></v-img>

            <v-card-title>
              Gengibre
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 ml-1' : ''">
            <v-img src="azeitealhoealecrim.jpg" height="200px" cover></v-img>

            <v-card-title>
              Alho/Alecrim
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 mr-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-0' : ''">
            <v-img src="azeitelimao.jpg" height="200px" cover></v-img>

            <v-card-title>
              Limão Siciliano
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 mr-2 ml-2 text-green-darken-4">ENCOMENDAR</v-btn>
          </v-card>
        </v-container>

        <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 mr-1' : 'w-0'">
            <v-img src="azeitealecrim.jpg" height="200px" cover></v-img>

            <v-card-title>
              Alecrim
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
            <v-img src="azeitelimao.jpg" height="200px" cover></v-img>

            <v-card-title>
              Limão Sicilia
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 mr-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

        </v-container>


        <v-container class="d-flex justify-space-between">
          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-0' : ''">
            <v-img src="azeitepimenta.jpg" height="200px" cover></v-img>

            <v-card-title>
              Pimenta
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 ml-2 text-green-darken-4">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 mr-1' : ''">
            <v-img src="azeitecebola.jpg" height="200px" cover></v-img>

            <v-card-title>
              Cebola
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 ml-1' : ''">
            <v-img src="azeitehortela.png" height="200px" cover></v-img>

            <v-card-title>
              Hortelã
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 mr-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-0' : ''">
            <v-img src="azeitelaranja.jpg" height="200px" cover></v-img>

            <v-card-title>
              Laranja
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 mr-2 ml-2 text-green-darken-4">ENCOMENDAR</v-btn>
          </v-card>
        </v-container>

        <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 mr-1' : 'w-0'">
            <v-img src="azeitepimenta.jpg" height="200px" cover></v-img>

            <v-card-title>
              Pimenta
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>

          <v-card width="200" class="elevation-24 bg-green-darken-4" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
            <v-img src="azeitelaranja.jpg" height="200px" cover></v-img>

            <v-card-title>
              Laranja
            </v-card-title>

            <v-card-subtitle>
              <h2>R$ 24,90</h2>
            </v-card-subtitle>

            <v-btn class="bg-white mt-4 mb-2 mr-2 ml-2 text-green-darken-4"
              :class="smAndDown ? 'pl-1 pr-1' : ''">ENCOMENDAR</v-btn>
          </v-card>
        </v-container>
      </v-container>
    </v-img>


    <v-footer class="bg-green-darken-4 align-center justify-center">

      <div class="align-center justify-center w-25">
        <h1 class="font mt-5 mb-2 text-black" :class="smAndDown ? 'mb-10 pt-2' : ''">Flecha Sabores</h1>
        <div :class="smAndDown ? 'w-0 h-0 white' : ''">
          <h5 :class="smAndDown ? 'pt-2' : ''">Estamos comprometidos com a sua saúde, a saúde do planeta e, é
            claro, o prazer
            de uma refeição deliciosa. Aproveite nossos produtos e comece a sua jornada para uma vida mais saudável e
            saborosa.<p></p>
            <span class="text-black">Gratidão em ter você conosco!</span></h5>
        </div>
      </div>



      <div class="align-center justify-center ml-16">

        <v-chip>
          <svg-icon color="black" type="mdi" :path="path"></svg-icon>
          <h4 class="ml-3">(84) 999584725</h4>
        </v-chip>

        <br>

        <v-chip class="mt-5">
          <svg-icon color="black" type="mdi" :path="path1"></svg-icon>
          <h4 class="ml-3">Flecha Sabores</h4>
        </v-chip>

      </div>
    </v-footer>

    <div class="bg-white w-100 d-flex align-center justify-center">
      <v-chip color="black" class=" mt-3 mb-3" href="https://github.com/luanmello777" target="_blank>"><svg-icon type="mdi"
          :path="path2" class="mr-2"></svg-icon>github.com/Luanmello777
      </v-chip>
    </div>

  </v-app>
</template>

<style scoped>
.cont1 {
  border-color: #1B5E20;
  border-width: 10px;
  border-top-width: 0px;
  border-bottom: 0px;
  border-top-color: white;
}

.borda1 {
  border-color: white;
  border-width: 2px;
}

.card1 {
  border-color: #1B5E20;
  border-width: 2px;
}
</style>

<script setup>
import { useDisplay } from 'vuetify';
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiWhatsapp, mdiInstagram, mdiGithub } from '@mdi/js';

const { smAndDown } = useDisplay()
const path = mdiWhatsapp;
const path1 = mdiInstagram;
const path2 = mdiGithub;
</script>
