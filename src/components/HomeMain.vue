<template>
  <router-link to="/Reservas"><button class="botaoreserva"> Reserve já ! </button> </router-link>
  <main>    
    <section class="sec">
      <div>
        <h2>BEM-VINDO</h2>        
        <p>
        No Hotel Casa de Praia, você desfruta de uma das mais belas praias do Litoral Norte de São Paulo,
        alinhando conforto e diversão com paisagens únicas das praias locais e a tranquilidade do nosso
        Hotel.
        Para maior comodidade, oferecemos estacionamento interno com cerca de 40 vagas, piscinas, salão de
        festas e muito mais.
        </p>
        <p>
          Somos uma empresa de hotéis boutique com paixão por fornecer serviços de qualidade. 
          Orgulhamo-nos do serviço ao cliente e queremos tornar a sua estadia a melhor possível.
        </p>
      </div>
      
      <MainServicos/>
      <MainGastronomia/>
      <MainAcomodacoes/>
      <br>
      <hr>
      <MainMural/>
      <div>     
        <h3>Nossa Localização</h3>
        <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3659.187389827689!2d-45.0746653!3d-23.489759!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x94cd57471e9de3c7%3A0x6d421826e100f11b!2sHOTEL%20CASA%20NA%20PRAIA!5e0!3m2!1spt-BR!2sbr!4v1664833770590!5m2!1spt-BR!2sbr"
        width="300" height="150" style="border:0;" allowfullscreen="" loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"></iframe>
      </div>
    </section>
  </main>
</template>

<script>

import MainMural from './home/MainMural'
import MainGastronomia from './home/MainGastronomia'
import MainServicos from './home/MainServicos'
import MainAcomodacoes from './home/MainAcomodacoes'


export default {
  name: 'HomeMain',
  components: { 
    MainMural,
    MainGastronomia,
    MainServicos,
    MainAcomodacoes,
    
  }
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@charset "UTF-8";
@import url("https://fonts.googleapis.com/css?family=Poppins:300,400,500,600,700,800,900&display=swap");
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
}

.sec {
  position: relative;
  padding: 2vw;
  background-color: #f4f2e7;
  background-image: linear-gradient(90deg, #f4f2e7 0%, #f7f4e9 46%, #efe5d5 100%);
  transition: all 0.3s ease;
  color: black;
}

.sec > div{
  max-width: 90%;
  margin: 2% 5%; 
}
.sec h2 {
  font-size: 3em;
}

.sec h3,
.sec h4 {
  margin-bottom: 0.5em;
  margin-top: 0.5em;
}

.sec p {
  font-size: 1.2em;
  font-weight: 300;
}

.sec iframe {
  width: 35vw;
  display: flex;
  flex-direction: column;
  justify-content: left;
  align-items: left;
}

img{
  max-width: 50%;
  display: block;
  border-radius: 20px;
  border: 3px solid blue;
}


.botaoreserva {
  position: fixed;
  left: 93%;
  top: 40%;
  font-weight: bold;
  font-size: 1em;
  background-color: rgb(89, 0, 255);
  color: rgb(240, 241, 245);
  border-radius: 5em;
  border: none;
  padding: 1em 1em 1em 1em;
  cursor: pointer;
  z-index: 9999;
}

.botaoreserva:hover {
  transform: translate(0px, -2px);
  -webkit-box-shadow: 0px 10px 7px -9px rgba(0, 0, 0, 0.75);
  -moz-box-shadow: 0px 10px 7px -9px rgba(0, 0, 0, 0.75);
  box-shadow: 0px 10px 7px -9px rgba(0, 0, 0, 0.75);
  transition: all 0.3s ease-out;
}

</style>
