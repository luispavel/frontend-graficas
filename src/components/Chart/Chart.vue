<template>
    <v-container fluid>
        <vc-donut
    background="white" 
    foreground="#EEEEEE"
    :size="200" 
    unit="px" 
    :thickness="10"
    :start-angle="0"
    :has-legend="false" 
    legend-placement="bottom"
    :sections="sections" 
    :total="100"
    :auto-adjust-text-size="true"
    >
    <h3> {{ tituloChart }} </h3>
    <h4> {{ cantChart }} </h4>
  </vc-donut>
    </v-container>
</template>
<script>
  export default {
    name: "Chart",
    data() {
      return {
        // sections: [
        //   {  label: 'Red section', value: 40, color: '#56A3A6' },
        //   {  label: 'Green section', value: 60, color: '#114B5F' },
        // ]
      };
    },
   props:{
       sections: [],
       tituloChart: String,
       cantChart: String,
       val1Chart: Number,
       val2Chart: Number
   },
    methods: {
      
    }
  };
</script>