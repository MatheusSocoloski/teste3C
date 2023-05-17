<template>
    <div class="div-text">
    <img  v-bind:src="imagem">
    <h2>{{ textPrincipal }}</h2>
    <p class="subtext"> {{ subText }}</p>
    <btn v-if="MostrarBotão" @click="mudar(); post()"></btn>
    <btn2 v-if="MostrarBotão2" @click="mudar(); post()"></btn2>
   
</div>


</template>

<script>
import axios from 'axios';
import btn from './btn.vue';
import btn2 from './btn2.vue';

export default {
  name: 'semVip',

  data() {
    return {
      textPrincipal: "Quer ter acesso antecipado ao Whatsapp da 3C Plus",
      subText: "O Whatsapp da 3C Plus está chegando e você pode entrar para a lista de primeiros usuários",
      textPrincipalVip: "Você já está na lista VIP do Whatsapp da 3C Plus",
      subTextPrincipalVip: "Nosso time entrará em contato em breve para mais informações",
      imagem: ['https://imgcloud.com.br/share/ycG0dgYALi14tf5i'],
      imagemVip: ['https://imgcloud.com.br/share/HlGDTZW9FVs5Ywuv'],
      MostrarBotão: true,
      MostrarBotão2: true
    };
  },
  components: {
    btn,
    btn2
  },
  methods: {
    mudar() {
      this.textPrincipal = this.textPrincipalVip;
      this.subText = this.subTextPrincipalVip;
      this.imagem = this.imagemVip;
      // this.btn = this.btnVip; // Verifique se btnVip está definido corretamente
      this.MostrarBotão = false;
      this.MostrarBotão2 = false;
    },
    post() {
      const message = 'Teste_pratico3C de Matheus Socoloski';

      axios
        .post('https://3cvoice.staging.3cplus.com.br/api/v1/user_data/557?api_token=CMi5xqN01dlrSAbm5pKerw7xmSAwF8HGlkwnTypdKMfJgxKocmI5unqK3srh', { message })
        .then(response => {
          console.log('Sucesso:', response.data);
        })
        .catch(error => {
          console.error('Erro:', error);
        });
        }
    }
}
</script>



<style  scoped>

h2{
    width: 433px;
    height: 76px;

    /* H1/32px Med */

    font-family: 'Cerebri Sans Pro';
    font-style: normal;
    font-weight: 500;
    font-size: 32px;
    line-height: 38px;
    /* or 119% */

    letter-spacing: -0.02em;

    /* Light/Text/Text 300 */

    color: #1B1B2B;


    /* Inside auto layout */

    flex: none;
    order: 0;
    flex-grow: 0;

}

.div-text{
    position: absolute;
    width: 433px;
    height: 281px;
    left: 489px;
    top: 240px;

}

.subText{
    
    width: 385px;
    height: 44px;

    /* H4/18px Reg */

    font-family: 'Cerebri Sans Pro';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 22px;
    /* or 122% */

    letter-spacing: -0.02em;

    /* Light/Text/Text 200 */

    color: #373753;


    /* Inside auto layout */

    flex: none;
    order: 1;
    flex-grow: 0;
    }
    .imgWppBlue{
   /* whatsapp */


    width: 45px;
    height: 45px;


/* Inside auto layout */

    flex: none;
    order: 0;
    flex-grow: 0;
}




</style>

    