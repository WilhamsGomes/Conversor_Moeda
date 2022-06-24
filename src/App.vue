<template>
    <div id="app">
      <h1>Conversor de moedas</h1>
      <div class="linha">
         <ConversorMoeda moeda-a="USD" moeda-b="BRL"/>
         <ConversorMoeda moeda-a="BRL" moeda-b="USD"/>
      </div>
      <div class="linha">
         <ConversorMoeda moeda-a="CAD" moeda-b="BRL"/>
         <ConversorMoeda moeda-a="BRL" moeda-b="CAD"/>
      </div>
      <div class="linha">
         <ConversorMoeda moeda-a="EUR" moeda-b="BRL"/>
         <ConversorMoeda moeda-a="BRL" moeda-b="EUR"/>
      </div>
      
    </div>
</template>

<script>

  import ConversorMoeda from './components/Conversor.vue'

  export default {
    name: 'App',
    components: {
      ConversorMoeda
    } 
  }
</script>

<style scoped>

  #app{
    margin: auto;
    max-width: 900px;
    text-align: center;
  }
  .linha{
    margin-top: 40px;
    display: flex;
    justify-content: space-around;
  }
</style>
