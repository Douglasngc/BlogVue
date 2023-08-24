<template>
  <div>
    <div class="gaps" v-for="post in posts" :key="post.img">
      <div class="line">
        <img v-bind:src="post.img" alt="ponto">
        <h2>{{ post.title }}</h2>
        <p>{{ post.post }}</p>
       
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FirstT',
  data() {
    return{
      
    nome: 'dg',
    posts:[{
      img:"../assets/equipe.png",
      title:'post 1',
      post:`QUEM SOMOS
A NPX surgiu em 2010 para fornecer o que há de melhor em Telefonia IP. Desde então, trabalhamos focados, dia após dia, na consolidação de um conceito principal: Entender as necessidades de nossos clientes, buscando sempre superar suas expectativas e atingir o seu mais alto grau de satisfação.
   MISSÃO: Implementar tecnologia de ponta com profissionalismo e qualidade ímpar ao universo corporativo com o objetivo maior de proporcionar a melhor experiência possível de comunicação para nossos clientes

   VISÃO: Alcançar o reconhecimento de nossos clientes e parceiros como empresa referência em qualidade na área, prezando sempre pela confiabilidade e excelência no atendimento

   VALORES: Comprometimento, inovação, humildade, foco no cliente, ser ninja e sangue nos olhos`
    },{
    img:'../assets/aurora.svg',
      title:'post 2',
      post:`Plataforma criada com o intuito de facilitar e automatizar
o atendimento ao cliente com mais agilidade, organização
e eficiência. No qual possibilita que várias plataformas de
mensagem sejam direcionadas ao Aurora.`
    },{
      img:'../assets/nxp.png',
      title:'post 3',
      post:`Reduza seus custos com números 0800, atendendo somente por alguns segundos, retornando por um valor mais acessível`

    }]
  
    }
  }}
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
