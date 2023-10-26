<template>
  <div class="grid-container">
    <div class="grid-x grid-margin-x">
        <div class="cell small-12 medium-2 large-3">
            <the-lista-categorias-vue/>
        </div>

        <div class="cell small-12 medium-10 large-9">
            <the-lista-colores-vue/>
            <router-view/>
        </div>

    </div>
    
  </div>
</template>

<script>
import TheListaCategoriasVue from '@/components/categorias/TheListaCategorias.vue'
import TheListaColoresVue from '@/components/categorias/TheListaColores.vue'
export default {
    name: 'CategoriaPage',
    components: {
        TheListaCategoriasVue,
        TheListaColoresVue
    }
}
</script>

<style lang="scss" scoped>
    
</style>

