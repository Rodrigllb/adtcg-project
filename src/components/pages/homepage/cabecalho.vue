<template>
  <header>
    <!--Container da logo da igreja-->
    <div class="logo-adtcg">
      <img src="./../../../assets/logo/logo-adtcg.png" alt="logo da igreja assembleia">    
    </div>
    
    <!--Barra de navegação para dispositivos desktop ou superiores-->
    <nav>
      <ul>
        <li><a href="#">Inicio</a></li>
        <li><a href="#historiadaigreja">História</a></li>
        <li><a href="#lideranca">Lideres</a></li>
      </ul>
    </nav>


    <!--Menu quando estiver aberto em dispositivos de menor tamanho-->
    <div id="menu-aberto">
      <section>
        <img src="./../../../assets/icons/options/iconInicio.png" alt="Icone do inicio">
        <a href="#">Inicio</a>
      </section>
      <section>
        <img src="./../../../assets/icons/options/iconHisto.png" alt="Icone da historia da igreja">
        <a href="#">História</a>
      </section>
      <section>
        <img src="./../../../assets/icons/options/iconLideran.png" alt="Icone de liderança">
        <a href="#lideranca">Liderança</a>
      </section>
      <section class="marca">
        <small>Developed by Rodrigo Liberato - 2025</small>
      </section>
    </div>

    <!--Elemento para abrir menu em dispositivos mobile-->
    <img src="./../../../assets/icons/icon-menubar.png" id="abrir-menu" alt="icone para abrir menu">

  </header>  
</template>

<script>

export default { /*Exportando o elemento para o arquvio app.vue */
  name: 'cabecalhoSite'
  
}


document.addEventListener("DOMContentLoaded", function DOMcarregado() { //Espera o DOM ser completamente carregado para rodar o código abaixo.

  let exibirMenu = document.getElementById('abrir-menu');
  let menuExibido = document.getElementById('menu-aberto');

  if(exibirMenu) { //Verificar se o elemento no dom foi carregador corretamente.
    exibirMenu.addEventListener('click', () => {
      
        if(menuExibido.style.visibility === "hidden" || menuExibido.style.visibility === "") {
          menuExibido.style.visibility = 'visible'
          menuExibido.style.transition = 'ease 0.9s'
          menuExibido.style.transform = 'translateX(0px)'
        }
        else {
          menuExibido.style.visibility = 'hidden'
          menuExibido.style.transition = 'ease 2s'
          menuExibido.style.transform = 'translateX(1450px)'
        }

    });
    console.log('Elemento carregado com sucesso!');
  }
  else { //Se não carregar, o mesmo é exibido uma mensagem de erro no console do browser.
    console.error('Elemento não carregado!');
  }
});

</script>

<style scoped>
  header { /*Personalizações gerais do cabeçalho */
    display: grid;
    grid-template-columns: auto auto;
    align-items: center;
    justify-content: center;
    top: 0;
    z-index: 1;
    position: sticky;
    width: 100%;
    height: 85px;
    background-color: #131313;
    color: #ffff;
    box-shadow: rgba(0, 0, 0, 0.45) 0px 25px 20px -20px;
  }

  nav {
    margin-left: 25vh;
  }

  nav ul { /*Personalização referente aos links de navegação do cabeçalho */
    display: flex;
    flex-direction: row; 
    justify-content: space-around;
    align-items: center;
    width: 65vw;
    height: auto;
    list-style: none;
    font-weight: 300;
  }

  a { /*Estilização geral dos links */
    color: #fff;
    text-decoration: none;

  }


  /***BARRA DE MENU EM DISPOSITIVOS MOBILE***/
  #abrir-menu {
    display: none;
    border-radius: 7px;
  }

  #abrir-menu:hover {
    transition: all 0.9s;
    border: solid #fff 0.5px;
  }

  #menu-aberto {
    display: flex;
    position: fixed;
    visibility: hidden; 
    
    flex-direction: column;
    top: 85px;
    transform: translateX(550px);
    width: 100%;
    max-height: 70vh;
    margin: 0 auto;
    box-shadow: rgba(0, 0, 0, 0.45) 0px 25px 20px -20px;
    background-color: #5a5a5a;

  }
  #menu-aberto section {
    width: 100%;
    height: 55px;
    display: flex;
    align-items: center;
    flex-direction: row;
    padding-left: 12px;
  }
  #menu-aberto section:hover {
    background-color: #757575;
  }
  #menu-aberto section a {
    margin-left: 9px;
  }
  #menu-aberto section small {
    font-weight: 300;
    opacity: 75%;
    font-size: 12px;
  }
  #menu-aberto .marca {
    background-color: #3d3d3d;
  }



  /****RESPONSIVIDADE*****/
  

  @media (max-width: 1260px) {

    header {
      justify-content: space-between;
      padding: 0px 22px 0px 22px;
    }
    
    header nav {
      display: none;
    }

    #abrir-menu {
      display: flex;
    }

  }

</style>
