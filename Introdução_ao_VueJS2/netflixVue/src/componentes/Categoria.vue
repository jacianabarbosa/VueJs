<template>
  <div class="slider">
    <h3>{{titulo}}</h3>
    <span v-on:mouseover="scrollEsquerda()" v-on:mouseout="clearScroll()" class="handle handlePrev active">
        <i class="fa fa-caret-left" aria-hidden="true"></i>
    </span>

    <div ref="scroller" class="row">
       <div class="row__inner">
         <filme v-for="filme in filmes" v-bind:key="filme.id" v-bind:titulo="filme.titulo" v-bind:imagem="filme.imagem"></filme>
      </div>
    </div>
      
      <span v-on:mouseover="scrollDireita()" v-on:mouseout="clearScroll()"  class="handle handleNext active">
        <i class="fa fa-caret-right" aria-hidden="true"></i>
      </span>
  </div>

</template>

<script>
import Filme from './Filme.vue';

export default {
  props: ["titulo", "filmes"],
  components:{
      Filme
  },

  methods:{
    scrollDireita(){
        const self= this;
      this.intervalo = setInterval(function(){ self.$refs.scroller.scrollLeft += 1 }, 5);
    },
    scrollEsquerda(){
        const self= this;
      this.intervalo = setInterval(function(){ self.$refs.scroller.scrollLeft -= 1 }, 5);
    },
    clearScroll(){
        const self= this;
      clearInterval(this.intervalo);
    }
  }
}


</script>

<style lang="scss">
h3{
    color: white;
}
</style>
