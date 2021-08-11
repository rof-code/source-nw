<template>
    <main>
    <bannerProdutos/>
    <frete/>
    <kitProdutos/>
    <famososRecomendam/>
    <tabelaNutricional/>
    <depoimentos/>
    <compraSegura/>
    </main>
</template>


<script>
export default {
    components:{
         bannerProdutos: () => import(`@/components/gerais/bannerProdutos.vue`),
         frete: () => import(`@/components/gerais/frete.vue`),
         kitProdutos: () => import(`@/components/gerais/kitProdutos.vue`),
         famososRecomendam: () => import(`@/components/gerais/famososRecomendam.vue`),
         tabelaNutricional: () => import(`@/components/gerais/tabelaNutricional.vue`),
         depoimentos: () => import(`@/components/gerais/depoimentos.vue`),
         compraSegura: () => import(`@/components/gerais/compraSegura.vue`),
    }
}
</script>


<style lang="scss">
.imgResponsive{
    max-width:100%;
}
.kitProdutos .titleSection{
    display: none !important;
}
section.famosos{
    margin:30px 0px 60px 0px;
}
@media screen and (max-width: 850px){
.flickity-button{
    display:none !important;
}
.kitProdutos{
    padding:70px 0px 0px 0px !important;
}

}
</style>