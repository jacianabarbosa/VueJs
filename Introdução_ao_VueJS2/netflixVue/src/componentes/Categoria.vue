<template>
    <div class="slider">
      <h3>{{titulo}}</h3>
      <span v-on:mouseover="scrollEsquerda()" v-on:mouseout="clearScroll()" class="handle handlePrev active">
        <i class="fa fa-caret-left" aria-hidden="true"></i>
      </span>

      <div id="scroller" class="row">
        <div class="row__inner">
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="https://img1.ibxk.com.br/2015/11/12/12134915138723.jpg?w=700" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Assassin’s Creed
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="https://cdn.flickeringmyth.com/wp-content/uploads/2017/09/Thor-Ragnarok-banner-3-1-600x372.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Thor Ragnarok
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="https://s3.drafthouse.com/images/made/batmanvsuperman-xlarge_1050_591_81_s_c1.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Batmam versus Superman
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="https://www.blahcultural.com/wp-content/uploads/2017/06/mulher-maravilha-trailer-em-batalha-0-800x500.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Mulher Maravilha
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="https://static1.squarespace.com/static/51b3dc8ee4b051b96ceb10de/t/58c96236bf629a487883c763/1489592890396/" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Logan
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="http://cinemacomrapadura.com.br/imagens/2017/06/20170608-the-mummy-a-mumia-2017-tom-cruisi.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                A Múmia
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="http://www.oquerola.com/wp-content/uploads/2015/02/Imagem-do-Homem-Aranha-1024x640.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Homem-Aranha
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="https://static.independent.co.uk/s3fs-public/thumbnails/image/2017/02/03/15/transformers-the-last-knight.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Transformers: O último cavaleiro
              </div>
            </div>
          </div>
          <div class="gui-card">
            <div class="gui-card__media">
              <img class="gui-card__img" src="http://www.recifefm.com.br/wp-content/uploads/2017/06/piratas-do-caribe.jpg" alt=""  />
            </div>
            <div class="gui-card__details">
              <div class="gui-card__title">
                Assassin’s Creed
              </div>
            </div>
          </div>

        </div>
      </div>

      <span v-on:mouseover="scrollDireita()" v-on:mouseout="clearScroll()"  class="handle handleNext active">
        <i class="fa fa-caret-right" aria-hidden="true"></i>
      </span>

    </div>
</template>



<script>
    export default{
            props:['titulo']
        }
     
</script>

<style lang="scss">


</style>
