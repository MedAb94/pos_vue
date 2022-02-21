<template>
  <v-navigation-drawer app color="white" right width="290">
    <v-list subheader two-line class="mt-1">
      <v-list-item>
        <v-list-item-avatar rounded>
          <v-img src="https://cdn.vuetifyjs.com/images/lists/2.jpg"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title>Medab VALL</v-list-item-title>
          <v-list-item-subtitle>Responsible</v-list-item-subtitle>

        </v-list-item-content>
        <v-list-item-action>
          <v-badge bordered overlap color="red" dot>
            <v-icon>far fa-bell</v-icon>
          </v-badge>
        </v-list-item-action>
      </v-list-item>
    </v-list>
    <strong class="ml-3">Bills</strong>
    <v-list subheader two-line class="mt-1">
      <v-list-item>
        <v-list-item-avatar rounded color="grey lighten-4">
          <v-img src="2.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="subtitle-2">Riz</v-list-item-title>
          <v-list-item-subtitle>2 Kg</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action class="caption">30 MRU</v-list-item-action>
      </v-list-item>
    </v-list>
    <v-list subheader two-line class="mt-1">
      <v-list-item>
        <v-list-item-avatar rounded color="grey lighten-4">
          <v-img src="2.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="subtitle-2">Sucre</v-list-item-title>
          <v-list-item-subtitle>1 Kg</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action class="caption">15 MRU</v-list-item-action>
      </v-list-item>
    </v-list>
    <v-list subheader two-line class="mt-1">
      <v-list-item>
        <v-list-item-avatar rounded color="grey lighten-4">
          <v-img src="2.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="subtitle-2">Oil</v-list-item-title>
          <v-list-item-subtitle>1 L</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action class="caption">20 MRU</v-list-item-action>
      </v-list-item>
    </v-list>
    <v-list subheader two-line class="mt-1">
      <v-list-item>
        <v-list-item-avatar rounded color="grey lighten-4">
          <v-img src="2.png"></v-img>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title class="subtitle-2">Blé</v-list-item-title>
          <v-list-item-subtitle>2 Kg</v-list-item-subtitle>
        </v-list-item-content>
        <v-list-item-action class="caption">20 MRU</v-list-item-action>
      </v-list-item>
    </v-list>


    <v-divider class="mx-4"></v-divider>
    <v-toolbar color="rgba(0,0,0,0)" flat>
      <strong>Total</strong>
      <v-spacer></v-spacer>
      <strong>85 MRU</strong>
    </v-toolbar>

    <div class="mx-3 mt-2">
      <v-btn color="#704232" block dark class="widthoutupercase">Soumettre</v-btn>
    </div>
  </v-navigation-drawer>
</template>

<script>
export default {}
</script>

<style>
.v-card.borderme {
  border: 2px solid #704232 !important;
}

.col-12 {
  padding: 5px !important;
}

.v-btn.widthoutupercase {
  text-transform: none !important;
}
</style>