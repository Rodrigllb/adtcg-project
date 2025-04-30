    <template>
    <main>

        <article>
            <section class="fundo-igreja">
                <h1>Assembleia de Deus Templo Central do Gravier</h1>
                <p>Lugar de Restauração, Misericórdia e Ensino.</p>
            </section>

            <section class="links-rápidos">
                <div>
                    <a href="#"><img src="./../../../assets/icons/social/icongmail.png" alt="link para realizar envio de email"></a>
                    <a href="https://www.instagram.com/adtcgravier/" target="_blank"><img src="./../../../assets/icons/social/iconinsta.png" alt="link para o instagram da igreja"></a>
                    <a href="https://wa.link/e0m89j" target="_blank"><img src="./../../../assets/icons/social/iconwapp.png" alt="link para o whatsapp do pastor da igreja"></a>                        
                </div>
            </section>

            <section class="sobre-a-igreja">
                <div>
                    <h1>Uma comunidade, um corpo e um só Espírito.</h1>

                <p> Mais que um lugar, somos uma família.
                    Uma comunidade unida por um só Corpo, um só Espírito e um só propósito: viver e anunciar o amor de Cristo.
                    No Templo Central, acolhemos com carinho, acalentamos com fé e instruímos com a verdade da Palavra.
                    Aqui, cada vida importa. Cada coração encontra direção, consolo e propósito.
                    Somos guiados pelo Espírito Santo e firmados na única esperança de salvação: Jesus Cristo, o Caminho, a Verdade e a Vida.
                </p>
                </div>
                
                <div class="video-apresentativo">
                    <video width="480" height="894" controls>
                        <source src="./../../../assets/videos/video-igreja.mp4" >
                    </video>
                    <small>Aniversário em homenagem ao nosso Pastor</small>
                </div>
            </section>

            <section class="departamentos">
                
                <h3>Departamentos</h3>
                <small>União dos jovens, senhoras e crianças</small>
                
                <div>
                    <section>
                    <img src="./../../../assets/logo/umadgLogo.jpg" alt="União de mocidade">
                        <p>UMADG</p>
                    </section>
                    <section>
                        <img src="./../../../assets/logo/usadgLogo.jpg" alt="União de senhoras">
                        <p>USADG</p>
                    </section>
                    <section>
                        <img src="./../../../assets/logo/diadgLogo.jpg" alt="União de crianças">
                        <p>DIADG</p>
                    </section>
                </div>
            </section> 

            <section id="lideranca">
                <h3>Liderança</h3>
                <small>Pastor e Diáconos da igreja</small>

                <div class="lideres">
                    <section>
                        <img src="./../../../assets/lideres/diaconoclavesherique.webp" alt="Diacono">    
                        <p>Diácono Henrique</p>
                    </section>         

                    <section>
                        <img src="./../../../assets/lideres/prvaldecirecicera.webp" alt="Pastores">
                        <p>Pastor Valdecir</p>
                    </section>

                    <section>
                        <img src="./../../../assets/lideres/diaconobruno.webp" alt="Diacono">
                        <p>Diácono Bruno</p>
                    </section>

                </div>

            </section>

            <section id="historiadaigreja">

                <div>
                    <h1>Nossa história</h1>

                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Non maiores dolore, accusantium voluptates doloribus magnam voluptatibus fugiat fugit accusamus blanditiis qui laborum consequatur? Voluptatum veritatis atque reprehenderit nesciunt! Fugiat, omnis.
                    </p>
                </div>

            </section>

        </article>

    </main>
</template>

<script>
    export default {
        name: 'corpoSite'
    }

</script>

<style scoped>

    main article { /*Estilização do corpo do site*/
        display: flex;
        flex-direction: column;
        width: 100%;
        min-height: 100vh;
    }

    .fundo-igreja { /*Estilização da seção referente ao fundo da imagem da igreja*/
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        text-align: center;
        height: 500px;
        width: 100%;
        color: #fff;
        padding: 12px;
        background-image: url('./../../../assets/backgrounds/fundoigrejadesktop.webp');
        background-repeat: no-repeat;
        background-size: cover;
    } 
    .fundo-igreja h1 {
        font-size: 38px;
    }

    .links-rápidos {
        display: flex;
        flex-direction: row;
        align-items: center;
        width: 100%;
        height: 120px;
        background-color: #252525;
    }
    .links-rápidos div {
        display: flex;
        justify-content: space-around;
        width: 550px;
        height: auto;
        margin: 0 auto;
    }
    .links-rápidos div img:hover {
        transition: all 0.7s ease-in-out;
        transform: translateY(-12px);
    }

    .sobre-a-igreja { /*Container referente a descrição da igreja */
        display: grid;
        grid-template-columns: 756px auto;
        text-align: left;
        align-items: center;
        width: 100%;
        padding: 22px;
    }
    .sobre-a-igreja h1 {
        font-size: 38px;
        font-weight: 900;
    }
    .sobre-a-igreja h2 {
        font-size: 30px;
        padding-bottom: 12px;
    }
    .sobre-a-igreja p {
        padding-bottom: 12px;
        text-align: justify;
    }
    .sobre-a-igreja em {
        background-color: #e4e4e4;
    }
    
    .video-apresentativo { /*Container do video representativo*/
        display: flex;
        flex-direction: column;
        margin: 0 auto;
        width: 90%;
        height: auto;
        align-items: center;
        justify-content: center;    
    }
    .video-apresentativo video { /*Estilização do video */
        width: 320px;
        height: 500px;
        border-radius: 15px;
        background-color: #101010;
    }
    .video-apresentativo small {
        font-size: 12px;
        font-weight: 300;
        opacity: 80%;
    }

    .departamentos { /*Estilização do container dos departamentos */
        display: flex;
        flex-direction: column;
        width: 100%;
        height: auto;
        background-color: #c4c4c4; 
        padding-top: 22px;
        padding-bottom: 22px;   
    }
    .departamentos h3 { /*Estilização especifica do titulo nivel três dentro desse container */
        font-size: 35px;
    }
    .departamentos div { /*Estilização geral do elementos div's do container departamentos */
        display: flex;
        justify-content: space-around;
        flex-direction: row;
        padding: 42px;
    }
    .departamentos section { /*Estilização das seções */
        justify-content: center;
        align-items: center;
        width: 35vh;
        height: 15vh;
        border-radius: 25px;
    }
    .departamentos section img { /*Estilização das imagens dentro das seções dos departamentos */
        width: 75px;
        height: auto;
        border: solid 2px #252525;
        border-radius: 50%;
    }

    #lideranca {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: auto;
        background-color: #101010;
        color: #e4e4e4;
        padding-top: 22px;
    }
    #lideranca h3 {
        font-size: 35px;
    }
    .lideres {
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        align-items: center;
        width: 100%;
        height: 250px;
        padding: 5px;
    }
    .lideres section {
        justify-content: center;
        align-items: center;

    }
    .lideres small {
        font-size: 9px;
        font-weight: 600;
    }
    .lideres img {
        width: 85px;
        height: auto;
        border: 2px solid #e4e4e4;
        border-radius: 50%;
        margin: 12px;
    }


    #historiadaigreja { /*Historia sobre a igreja*/
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        text-align: justify;
        padding: 22px;
        width: 100%;
        height: auto;
    }
    #historiadaigreja h1 {
        font-size: 38px;
    }




    /****RESPONSIVIDADE****/

    @media (max-width: 1260px) {

        main article {

        }

        .sobre-a-igreja {
            display: grid;
            grid-template-columns: 100%;
        }


        .video-apresentativo {
            display: flex;
        }
        .video-apresentativo video {
            width: 100%;
            height: 200px;
        }
    }


    @media (max-width:  740px) {
        main article {

        }

        .fundo-igreja {
            display: flex;
            color: #fff;
            background-image: url('./../../../assets/backgrounds/background-igreja.jpg');
            background-repeat: no-repeat;
            background-size: cover;
        }

    }

</style>