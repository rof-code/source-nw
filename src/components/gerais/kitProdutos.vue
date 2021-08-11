<template>
    <section class="kitProdutos">
        <div class="container">
            <div class="titleSection text-center">
                <h1>Escolha seu tratamento</h1>
                <p>Compre agora e tenha dentes brancos <br class="mob"> em até 14 dias!</p>
            </div>
            <div class="row justify-content-center">
                
                <div class="col-sm-5 bloco2" id="bloco2">
                    <div class="col-sm-12 mainContent"
                    style="
                        border-radius:25px;
                        box-shadow:0px 10px 30px rgba(0,0,0,0.6);
                        border:1px solid #FF6E04;
                        text-align:center;
                        ">

                        <div class="col-sm-12 colTitulo"
                        style="
                            border-top-left-radius:20px;
                            border-top-right-radius:20px;
                            background-color:#FF6E04;
                        ">
                            <p>Compre 2 Leve 4</p>
                            <p>#semanadosorrisobranco</p>
                        </div><!--col--titulo-->
                        <div class="col-sm-12 colImagem">
                            <img class="imgResponsive" src="@/assets/newwhite/new-white-combo-2potes-2creme-dental.png" alt="newwhite Be 1 Pote - Vitabe" id="param2" style="margin:30px 0px;">
                            <p style="margin-top:-10px;margin-bottom:20px;"><strong>Promoção:</strong>Compre 2 Leve 4</p>
                            <div class="flag-frete">
                                <img src="@/assets/newwhite/flag-frete-gratis-new-white.gif" alt="Frete Grátis newwhite Be"
                                style="
                                position:absolute;
                                top:10%;
                                right:5%;">
                            </div>
                        </div><!--col-da-imagem-->

                        <div class="relogio" style="background-color:#FF6E04;margin-bottom:15px;">
                            <div class="col-12 d-flex align-items-center" style="padding:7px 0px 2px 0px;">
                                <div class="col-4" style="position:relative;right:-13%;">
                                    <img src="@/assets/newwhite/relogio.png" alt="" style="top:-3px;position: relative;">
                                </div>
                                <div class="col-8" style="color:#fff;position:relative;left:-10%;">
                                    <p style="margin-bottom:0px;font-weight:bold;font-size:14px;">OFERTA EXPIRA EM:</p>
                                    <p id="crono" style="margin-bottom:0px;font-size:34px;font-weight:bold;"></p>
                                </div>
                            </div>
                        </div><!--div do relógio-->


                        <div class="col-sm-12">
                            <p style="color:#8f8f8f;font-size:18px;margin-bottom:0px;">Preço tabela: <s><strong> R$ 359,80</strong></s></p>
                            <p style="color:#8f8f8f;font-size:18px;margin-bottom:0px;">Preço promocional: <strong style="color:#000;"> R$ 167,70</strong></p>
                            <img src="@/assets/newwhite/img-ou.png" class="imgResponsive" alt="">
                            <p style="color:#8f8f8f;font-size:18px;margin-bottom:0px;">12x sem juros de</p>
                            <span style="color:#000;font-weight:700;font-size:45px;font-family: 'Helvetica',sans-serif;display:block;">R$ 13,98</span>
                            <input type="submit" value="COMPRE AGORA" class="btnComprar" @click="addCartBoxCompra1()">
                            <img class="imgResponsive ico-frete" src="@/assets/newwhite/ico-frete-gratis.png" alt="">
                        </div><!--col-do-preço-->
                    </div><!--container--geral-->
                </div><!--bloco2-->


                <div class="col-sm-5 bloco1" id="bloco1">
                    <div class="col-sm-12 mainContent"
                    style="
                        border-radius:25px;
                        box-shadow:0px 10px 30px rgba(0,0,0,0.6);
                        border:1px solid #e7e7e7;
                        text-align:center;
                        ">

                        <div class="col-sm-12 colTitulo"
                        style="
                            border-top-left-radius:20px;
                            border-top-right-radius:20px;
                            background-color:#e7e7e7;
                        ">
                            <p style="color:#000;">Compre 1 Leve 2</p>
                            <p style="color:#000;">Sorriso branco em até 14 dias</p>
                        </div><!--col--titulo-->

                        <div class="col-sm-12 colImagem">
                            <img class="imgResponsive" :src="require('@/assets/newwhite/new-white-combo-1pote-1creme-dental.png')" alt="New white" id="param" style="margin:42px 0px;">
                            <p style="color: #000;font-size: 18px;margin-top: 20px;font-weight: 300;margin-bottom:20px;">Contém: 1 Pote Clareador Dental + <br>
                            Creme Dental New White</p>
                            <div class="flag-frete">
                                <img src="@/assets/newwhite/flag-frete-gratis-new-white.gif" alt="Frete Grátis New White "
                                style="
                                position:absolute;
                                top:5%;
                                right:5%;">
                            </div>
                        </div><!--col-da-imagem-->

                        <div class="col-sm-12">
                            <p style="color:#8f8f8f;font-size:18px;margin-bottom:0px;">Preço tabela: <s><strong> R$ 119,90</strong></s></p>
                            <p style="color:#8f8f8f;font-size:18px;margin-bottom:0px;">Preço promocional: <strong style="color:#000;"> R$ 94,70</strong></p>
                            <img src="@/assets/newwhite/img-ou.png" class="imgResponsive" alt="">
                            <p style="color:#8f8f8f;font-size:18px;margin-bottom:0px;">12x sem juros de</p>
                            <span style="color:#000;font-weight:700;font-size:45px;font-family: 'Helvetica',sans-serif;">R$ 7,89</span>

                            <input type="submit" value="COMPRE AGORA" class="btnComprar" @click="addCartBoxCompra()">
                            <img class="imgResponsive ico-frete" src="@/assets/newwhite/ico-frete-gratis.png" alt="">
                        </div><!--col-do-preço-->
                    </div><!--container--geral-->
                </div><!--bloco1-->

            </div><!--row-->
        </div><!--container-->
    </section>
</template>

<script>
import Comunicacao from '@/comunicacao.js'
export default {
    mounted(){
        // CRONOMETRO

        // Set the date we're counting down to
        var countDownDate = new Date("jan 29, 2022 23:59:59").getTime();
        // Update the count down every 1 second
        var x = setInterval(function() {
        // Get today's date and time
        var now = new Date().getTime();
        // Find the distance between now and the count down date
        var distance = countDownDate - now;
        // Time calculations for days, hours, minutes and seconds
        var days = Math.floor(distance / (1000 * 60 * 60 * 24));
        var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
        var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60));
        var seconds = Math.floor((distance % (1000 * 60)) / 1000);
        var daybr = days;
        console.log(daybr);
        const textoHoras = (`00${hours}`).slice(-2);
        const textoMinutos = (`00${minutes}`).slice(-2);
        const textosegundos = (`00${seconds}`).slice(-2);

        // Display the result in the element with id="demo"
        document.getElementById("crono").innerHTML = textoHoras + ":"
        + textoMinutos + ":" + textosegundos;

        // document.getElementById("crono1").innerHTML = textoHoras + ":"
        // + textoMinutos + ":" + textosegundos;

        // document.getElementById("crono2").innerHTML = textoHoras + ":"
        // + textoMinutos + ":" + textosegundos;

        // If the count down is finished, write some text
        if (distance < 0) {
            clearInterval(x);
            document.getElementById("demo").innerHTML = "EXPIRED";
        }
        }, 1000);
        // CRONOMETRO
    },
    data(){ 
        return {
        boxCompraCarrinho: {
        tipo: "produto",
        itens: [
        {
            idProduto: "39",
            idAtributoSimples: "0",
            idUnidadeVenda: "0",
            idArmazem: "0",
            quantidade: "1",
            adicional: "",
            parametros: ""
        },
        {
            idProduto: "40",
            idAtributoSimples: "0",
            idUnidadeVenda: "0",
            idArmazem: "0",
            quantidade: "1",
            adicional: "",
            parametros: ""
        }
        ]
        },
        boxCompraCarrinho1: {
        tipo: "produto",
        itens: [
        {
            idProduto: "41",
            idAtributoSimples: "0",
            idUnidadeVenda: "0",
            idArmazem: "0",
            quantidade: "1",
            adicional: "",
            parametros: ""
        },
        {
            idProduto: "42",
            idAtributoSimples: "0",
            idUnidadeVenda: "0",
            idArmazem: "0",
            quantidade: "1",
            adicional: "",
            parametros: ""
        },
        ]
        },
        boxCompraCarrinho2: {
        tipo: "produto",
        itens: [
        {
        idProduto: "41",
        idAtributoSimples: "0",
        idUnidadeVenda: "0",
        idArmazem: "0",
        quantidade: "1",
        adicional: "",
        parametros: ""
        }
        ]
        },
    }
    },
    components:{

    },
    methods: {
    addCartBoxCompra() {
      Comunicacao.$emit('toggleLoader', true);
      let {tipo, itens} = this.boxCompraCarrinho;
      let itemAdc       = false
      if (tipo && itens) {
        //ADICIONA O PRODUTO AO CARRINHO
        this.$carrinho.add(tipo,itens,(success, response) => {
          response.data.itens.forEach(prod => {
            itemAdc = itemAdc ? itemAdc : prod.hash.idProduto == this.boxCompraCarrinho.itens[0].idProduto;
          });
          //PRODUTO ADICIONADO COM SUCESSO
          if(success) return Comunicacao.$emit('toggleCarrinho', {show: true, data: response.data });
          //PROBLEMAS AO ADICIONAR PRODUTO
          alert('Um problema impediu a adição do produto ao carrinho. Tente novamente mais tarde.');
        });
        return;
      }
    },
    addCartBoxCompra1() {
      Comunicacao.$emit('toggleLoader', true);
      let {tipo, itens} = this.boxCompraCarrinho1;
      let itemAdc       = false
      if (tipo && itens) {
        //ADICIONA O PRODUTO AO CARRINHO
        this.$carrinho.add(tipo,itens,(success, response) => {
          response.data.itens.forEach(prod => {
            itemAdc = itemAdc ? itemAdc : prod.hash.idProduto == this.boxCompraCarrinho1.itens[0].idProduto;
          });
          //PRODUTO ADICIONADO COM SUCESSO
          if(success) return Comunicacao.$emit('toggleCarrinho', {show: true, data: response.data });
          //PROBLEMAS AO ADICIONAR PRODUTO
          alert('Um problema impediu a adição do produto ao carrinho. Tente novamente mais tarde.');
        });
        return;
      }
    },
    addCartBoxCompra2() {
      Comunicacao.$emit('toggleLoader', true);
      let {tipo, itens} = this.boxCompraCarrinho2;
      let itemAdc       = false
      if (tipo && itens) {
        //ADICIONA O PRODUTO AO CARRINHO
        this.$carrinho.add(tipo,itens,(success, response) => {
          response.data.itens.forEach(prod => {
            itemAdc = itemAdc ? itemAdc : prod.hash.idProduto == this.boxCompraCarrinho2.itens[0].idProduto;
          });
          //PRODUTO ADICIONADO COM SUCESSO
          if(success) return Comunicacao.$emit('toggleCarrinho', {show: true, data: response.data });
          //PROBLEMAS AO ADICIONAR PRODUTO
          alert('Um problema impediu a adição do produto ao carrinho. Tente novamente mais tarde.');
        });
        return;
      }
    },
    }
}
</script>

<style lang="scss" scoped>
    .kitProdutos{
        input.btnComprar{
            display:block;
            margin:0 auto;
        }
        .ico-frete{
            max-width:100% !important;
        }
        .optionnewwhite{
            padding: 10px 26px;
            margin: 10px 0px 20px 0px;
            min-width:230px !important;
            max-width:230px !important;
        }
        .mainContent{
            padding:0px;
        }
        .titleSection{
            margin-bottom:30px;
        }
        padding:30px 0px;
        .colTitulo{
            padding:15px 0;
        }
        .colTitulo p:first-child{
            color:#fff;
            font-size:30px;
            font-weight:bold;
        }
        .colTitulo p:last-child{
            color:#fff;
        }
        .maisVendido{
            font-weight: bold;
            color:#f13787;
        }
        .maisVendido i{
            color:#f13787;
            margin:0px 15px
        }
        .imgResponsive{
            max-width: 100%;
        }
        .btnComprar{
            background-color:#04b900;
            color:#fff;
            font-weight: bold;
            width:200px;
            height:60px;
            border-radius:6px;
            font-family: 'Helvetica',sans-serif;
            border:none;
            cursor: pointer;
            transition: 0.4s ease;
        }
        .btnComprar:hover{
            opacity: 0.8;
        }
        .ico-frete{
            margin:20px 0px 30px 0px;
        }
    }
    @media screen and (max-width: 768px){
        
        .bloco1,
        .bloco2,
        .bloco3{
            margin:0px 0px 50px 0px !important;
        }
    }
</style>