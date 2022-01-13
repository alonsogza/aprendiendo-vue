<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>{{ texto }}</h2>
    <div style="background: #ffa150">
      <p> Desde el componente <strong>[HelloWrod]</strong> cargamos el otro componente <strong>[MiComponete]</strong> </p>
      <MiComponente></MiComponente>
    </div>
  </div>
</template>

<script>
// Para usar "MiComponente" en el componente de HelloWord se requiere importar "MiComponente"
import MiComponente from "./MiComponente.vue"

export default {
  name: 'HelloWorld',
  components: {  // Despues se agrega en COMPONENTS
    MiComponente,
  },
  props: {
    msg: String
  },
  // ** Con la DATA enviamos informacion para enlazar el HTML ( TEMPLEATE ) con datos JS, en este ejemplo ponemos TEXTO
  data(){     
    return{
      texto: "Hola Mundo desde el componente HelloWord"
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
