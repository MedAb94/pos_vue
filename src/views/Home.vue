<template>
  <v-app :style="{background: $vuetify.theme.themes.dark.background}">

    <v-container>
      <v-toolbar color="rgba(0,0,0,0)" flat>
        <v-toolbar-title class="mt-n3">Choisir un produit</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-text-field label="Rechercher un produit..."
                      class="mt-5"
                      color="brown"
                      filled append-icon="mdi-magnify"
                      dense solo flat background-color="grey lighten-4"></v-text-field>
      </v-toolbar>
      <v-item-group mandatory class="mt-n1">
        <v-container>
          <v-row justify="center" class="space">
            <v-col cols="12"
                   md="3"
            >
              <v-item v-slot="{ active, toggle }">
                <v-card
                    :color="active ? '#F6EFEF' : 'white'"
                    :class="active ? 'borderme' : 'borderout'"
                    class="d-flex align-center rounded-lg mx-2"
                    dark
                    height="140"
                    @click="toggle"
                    flat
                >
                  <v-row>
                    <v-col cols="12" sm="12">
                      <v-list-item three-line class="text-center ">
                        <v-list-item-content>
                          <div align="center" justify="center">

                            <v-img src="wheat.png" max-height="110" max-width="110" contain></v-img>

                          </div>
                          <v-list-item-subtitle
                              :class="active ? 'brown--text' : 'black--text'" class=" caption mt-4">Blé
                          </v-list-item-subtitle>

                        </v-list-item-content>
                      </v-list-item>
                    </v-col>
                  </v-row>

                </v-card>
              </v-item>
            </v-col>
            <v-col
                cols="12"
                md="3"
            >
              <v-item v-slot="{ active, toggle }">
                <v-card
                    :color="active ? '#F6EFEF' : 'white'"
                    :class="active ? 'borderme' : 'borderout'"
                    class="d-flex align-center rounded-lg mx-2"
                    dark
                    height="140"
                    @click="toggle"
                    flat

                >
                  <v-row>
                    <v-col cols="12" sm="12">
                      <v-list-item three-line class="text-center ">
                        <v-list-item-content>
                          <div align="center" justify="center">

                            <v-img src="rice.png" max-height="90" max-width="90" contain></v-img>

                          </div>
                          <v-list-item-subtitle
                              :class="active ? 'brown--text' : 'black--text'" class=" caption mt-3">Riz
                          </v-list-item-subtitle>

                        </v-list-item-content>
                      </v-list-item>
                    </v-col>
                  </v-row>

                </v-card>
              </v-item>
            </v-col>
            <v-col
                cols="12"
                md="3"
            >
              <v-item v-slot="{ active, toggle }">
                <v-card
                    :color="active ? '#F6EFEF' : 'white'"
                    :class="active ? 'borderme' : 'borderout'"
                    class="d-flex align-center rounded-lg mx-2"
                    dark
                    height="140"
                    @click="toggle"
                    flat
                >
                  <v-row>
                    <v-col cols="12" sm="12">
                      <v-list-item three-line class="text-center ">
                        <v-list-item-content>
                          <div align="center" justify="center">

                            <v-img src="sugar.png" max-height="80" max-width="80" contain></v-img>

                          </div>
                          <v-list-item-subtitle
                              :class="active ? 'brown--text' : 'black--text'" class=" caption mt-2">Sucre
                          </v-list-item-subtitle>

                        </v-list-item-content>
                      </v-list-item>
                    </v-col>
                  </v-row>

                </v-card>
              </v-item>
            </v-col>
            <v-col
                cols="12"
                md="3"
            >
              <v-item v-slot="{ active, toggle }">
                <v-card
                    :color="active ? '#F6EFEF' : 'white'"
                    :class="active ? 'borderme' : 'borderout'"
                    class="d-flex align-center rounded-lg mx-2"
                    dark
                    height="140"
                    @click="toggle"
                    flat
                >
                  <v-row>
                    <v-col cols="12" sm="12">
                      <v-list-item three-line class="text-center ">
                        <v-list-item-content>
                          <div align="center" justify="center">

                            <v-img src="oil.png" max-height="80" max-width="80" contain></v-img>

                          </div>
                          <v-list-item-subtitle :class="active ? 'brown--text' : 'black--text'"
                                                class=" caption mt-2">Oil
                          </v-list-item-subtitle>

                        </v-list-item-content>
                      </v-list-item>
                    </v-col>
                  </v-row>

                </v-card>
              </v-item>
            </v-col>
          </v-row>
        </v-container>
      </v-item-group>
      <v-toolbar color="#EEEEEE" flat>
        <v-toolbar-title>Client</v-toolbar-title>
        <v-spacer></v-spacer>
        <span color="grey">12 ventes aujourd'hui</span>
      </v-toolbar>
      <v-row>
        <v-col cols="12" sm="6">
          <v-card
              flat class="rounded-lg mx-5"
          >
            <v-list-item three-line>
              <v-list-item-content>
                <v-list-item-title class="text-h5">
                  Choix du client
                </v-list-item-title>
                <v-list-item-subtitle class="mt-1">Caramel sytrup with coffee, milk, and whipped cream
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-card-text>
              <v-text-field placeholder="NNI"></v-text-field>
              <v-text-field placeholder="Numero"></v-text-field>
              <div class="mx-3 mt-5">
                <v-btn color="#704232" block dark class="widthoutupercase">Verifier</v-btn>
              </div>
            </v-card-text>

          </v-card>
        </v-col>
        <v-col cols="12" sm="6">
          <v-card
              flat class="rounded-lg mx-5"
          >
            <v-list-item three-line>
              <v-list-item-content>
                <v-list-item-title class="text-h5">
                  Quantité du jour
                </v-list-item-title>
                <v-list-item-subtitle class="mt-1">Sweet chocolate with coffee, milk, and whipped cream
                </v-list-item-subtitle>
              </v-list-item-content>
            </v-list-item>
            <v-card-text>
              <div>
                <strong>Riz </strong>
                <v-progress-linear
                    color="light-blue"
                    height="10"
                    value="10"
                    striped
                ></v-progress-linear>
                <br>
                <strong>Sucre </strong>
                <v-progress-linear
                    color="light-green darken-4"
                    height="10"
                    value="20"
                    striped
                ></v-progress-linear>
                <br>
                <strong>Oil </strong>
                <v-progress-linear
                    height="10"
                    value="45"
                    striped
                    color="lime"
                ></v-progress-linear>
                <br>
                <strong>Blé </strong>
                <v-progress-linear
                    value="60"
                    height="10"
                    striped
                    color="deep-orange"
                ></v-progress-linear>
              </div>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

  </v-app>
</template>

<script>
/*import SideBar from '../components/SideBar'
import SideBarRight from '../components/SideBarRight'*/

export default {
  name: 'Home',

  components: {
   /* SideBar,
    SideBarRight*/
  },
}
</script>
<style>
.v-card.borderme {
  border: 2px solid #704232 !important;
}

.v-card.borderout {
  border: 1px solid #BCAAA4 !important;
}
</style>
