<template>
    <div id="mi-componente">
        <hr>
        <h1>Hola, este es mi componente</h1>
        <h2>{{subtitulo}}</h2>
        <hr>
    </div>
</template>

<script>
export default {
    name:   'MiComponente',
    data() {
        return{
            subtitulo: 'Soy el Subtitulo de mi componente [MiComponente.vue]'

        }
    }
    
}
</script>