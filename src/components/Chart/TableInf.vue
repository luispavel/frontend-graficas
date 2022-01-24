<template>
<v-container fluid>
    <v-row>
        <v-col justify-start><b><span v-bind:class="text1class">Tablet</span></b></v-col>       
        <v-col></v-col>
        <v-col justify-end><b><span v-bind:class="text2class">Smartphone</span></b></v-col>
    </v-row>
    <v-row>
        <v-col><b>{{porcTabla1}}%</b></v-col>
        <v-col>{{cantTabla1}}</v-col>
        <v-col></v-col>
        <v-col><b>{{porcTabla2}}%</b></v-col>
        <v-col>{{cantTabla2}}</v-col>
    </v-row>
    <v-row>
      <v-col>
        <v-banner single-line></v-banner>
      </v-col>

    </v-row>
</v-container>
</template>


<script>
export default {
  name: "Table",
  data() {
    return {};
  },
  components: {
    
  },
  props:{
    text1class: String,
    text2class: String,
    porcTabla1: Number,
    porcTabla2: Number,
    cantTabla1: String,
    cantTabla2: String
  },
  methods: {

  },

};
</script>

<style scoped>
</style>