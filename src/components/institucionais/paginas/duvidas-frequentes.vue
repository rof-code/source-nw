<template lang="html">
  <section>
    <div class="duvidasContainer-topo">
      <h1 class="vitabe-t1"> Perguntas Frequentes </h1>
      <p class="vitabe-t2"> Veja as principais dúvidas dos nossos clientes. </p>
      <p class="vitabe-t2"> Caso ainda tenha alguma pergunta que não apontamos aqui, fale com um de nossos canais de atendimento. </p>
    </div>
    <div class="duvidasContainer">
      <div class="duvidasContainer-item" v-for=" (item, i) in itens " :key=" i ">
        <p class="institucional-t1" @click=" $slideToggle($refs[`faq${i}`][0]); $event.target.classList.toggle('ativo') ">
          {{ item.pergunta }}
          <i class="fa fa-caret-right"></i>
        </p>
        <div :ref=" `faq${i}` " class="duvidasContainer-item-text">
          <p v-html="item.resposta"></p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      itens: [
        {
          pergunta: "O que é New White?",
          resposta:
            "New White é um clareador dental composto somente por ingredientes naturais, completamente livre de aditivos químicos. New White retira manchas, sujeira e amarelado da superfície dos dentes, deixando-os mais claros, brilhantes e com uma aparência mais saudável. Clarear os dentes nunca foi tão prático e prazeroso!",
        },
        {
          pergunta: "O que é o Creme Dental New White?",
          resposta:
            "O Creme Dental New White é um complemento para otimizar seus resultados com o New White em pó durante o tratamento. Vale lembrar que utilizando somente ele, você não obterá o resultado de clareamento nos dentes. É necessário fazer o uso em conjunto durante todo o tratamento.",
        },
        {
          pergunta: "Quantas gramas vem em cada pote e quanto tempo dura?",
          resposta:
            "Cada pote de New White Clareador possui 11g e dura cerca de 6 meses. Os kits darão o mesmo resultado, a diferença é que você prolongará o tempo do clareamento fazendo a manutenção com o produto de acordo com o kit.",
        },
        {
          pergunta: "Clareia o dente amarelado por cigarro?",
          resposta:
            "SIM, o New White remove as manchas, o amarelado e as pigmentações causadas pelo hábito de fumar cigarros, charuto ou cachimbo.",
        },
        {
          pergunta: "Quanto tempo para perceber resultados? Posso escovar os dentes só com o New White?",
          resposta:
            "Muitos clientes apresentam resultados logo na primeira semana, mas isso varia de pessoa a pessoa. Por isso recomendamos o uso contínuo por 14 dias, duas vezes ao dia, para uma maior eficácia. Após esse período, usar na frequência que achar necessária para a manutenção dos benefícios. O recomendado é manter a escovação dos dentes para auxiliar no efeito do produto.",
        },
        {
          pergunta: "New White pode danificar o esmalte dos meus dentes?",
          resposta:
            "Não. New White possui RDA de cerca de 68 e não apresenta qualquer ameaça ao esmalte dos seus dentes, sendo menos abrasivo do que grande parte das pastas comerciais tradicionais, que apresentam índices de RDA que variam entre 90 e 150.",
        },
        {
          pergunta: "Por que em outro site esses mesmos kits estão mais baratos e aqui tão caro?",
          resposta:
            "A venda de New White só pode ser realizada através deste SITE OFICIAL. Evite falsificações e riscos à sua saúde. NÃO adquira produtos sem procedência e qualidade garantidas. Não nos responsabilizamos por compras realizadas em outros sites. ESTÁ TERMINANTEMENTE PROIBIDA a venda do New White no Mercado Livre, Americanas.com, Submarino e Shoptime.",
        },
        {
          pergunta: "Existe alguma contraindicação? Se eu parar de usar volto a ter meus dentes amarelos?",
          resposta:
            "Não. Todos os seus ingredientes são classificados como seguros, não possuindo nenhum tipo de restrição de uso ou efeitos colaterais. New White é um produto registrado dentro dos padrões exigidos pela ANVISA para venda sem necessidade de receita. Para prolongar o clareamento dental, é recomendado o uso do New White periodicamente para manter o efeito do produto.",
        },
        {
          pergunta: "New White causa sensibilidade nos dentes igual aos clareadores químicos tradicionais?",
          resposta:
            "Diferente dos clareadores tradicionais, New White não age na dentina, agindo gentilmente na superfície dos dentes. Por ser um pó extremamente fino e rico em minerais, New White contribui para a remineralização dental, ajudando em casos de sensibilidade como relatado por clientes.",
        },
        {
          pergunta: "Eu preciso parar de tomar café, vinho ou refrigerante durante o processo?",
          resposta:
            "Não! New White age superficialmente no esmalte dental e devido às propriedades naturais, é um excelente aspirador de teanina – a substância responsável por manchar os dentes contida nos alimentos de cor forte. Assim, você pode contar com New White para combater as manchas causadas por essas substâncias.",
        },

        {
          pergunta: "Como usar o produto?",
          resposta:
            "Com a escova úmida, retire o excesso de água e mergulhe as cerdas no pote. Escove os dentes gentilmente em pequenos círculos, mantendo a boca fechada, por cerca de 5 minutos. Após o uso, enxágue abundantemente e escove os dentes com um pouco do seu creme dental tradicional para uma limpeza completa.",
        },

        {
          pergunta: "Qual o sabor de New White?",
          resposta:
            "New White não possui gosto algum, marcado por um leve toque de menta no final.",
        },

        {
          pergunta: "Posso clarear meus dentes mesmo usando aparelho fixo?",
          resposta:
            "Sim, agora você pode clarear os dentes mesmo com aparelho! Inclusive, o uso de New White auxilia na remoção de sujeiras não limpas na escovação normal.",
        },

        {
          pergunta: "Possuo resina/porcelana. Posso usar New White?",
          resposta:
            "Sim. O New White promove o clareamento também em porcelana e resina, fazendo com que esses materiais voltem a ter suas cores originais, porém o clareamento é mais potente em dentes naturais.",
        },
      ],
    };
  },
};
</script>

<style lang="css" scoped>
section {
  margin-bottom: 90px;
}
.duvidasT1 {
  display: block;
  color: #444;
  font-size: 14px;
}
.duvidasContainer-topo {
  margin: 40px 0 0;
}
.institucional-t1 {
  border-bottom: 1px solid #dbdbdb;
}
.duvidasContainer {
  overflow: hidden;
  border-radius: 4px;
}
.duvidasContainer-item {
  padding: 10px 0 0;
  border-bottom: none;
}
.duvidasContainer-item-text {
  overflow: hidden;
  display: none;
}
.duvidasContainer-item-text p {
  font-size: 14px;
  display: block;
  color: #828282;
  text-align: justify;
  padding: 10px;
}
.institucional-t1 i {
  transition: 200ms;
}
.institucional-t1.ativo i {
  transform: rotate(90deg);
}
@media (max-width: 767px) {
  .institucional-t1 {
    font-size: 14px;
  }
  .duvidasContainer-topo {
    margin: 0;
  }
}
</style>