<template>
  <v-container fluid>
      <v-row md12>
          <v-col md3
             v-for="(circle, index) in data1"
             v-bind:key="index"
          >
            <chart
                v-bind:sections="circle.sections"
                v-bind:tituloChart="circle.tituloChart"
                v-bind:cantChart="circle.cantChart"
            ></chart>
            <table-inf
                v-bind:text1class="circle.text1class"
                v-bind:text2class="circle.text2class"
                v-bind:porcTabla1="circle.porcTabla1"
                v-bind:porcTabla2="circle.porcTabla2"
                v-bind:cantTabla1="circle.cantTabla1"
                v-bind:cantTabla2="circle.cantTabla2"
            />
            </v-col>
      </v-row>
  </v-container>
</template>

<script>
import Chart from "./Chart.vue";
import TableInf from './TableInf.vue';
import data1 from '../../data/data1.json'
export default {
  name: "GroupChart",
  data:() => ({
      //importando los datos del archivo json
      data1,
  }),
  components: {
    Chart,
    TableInf
  },
  methods:{},
};
</script>

<style scoped>
</style>