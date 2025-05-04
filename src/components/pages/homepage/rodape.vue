<template>
    <footer>
        <div class="linksrodape">
            <ul>
                <li><a href="https://wa.link/e0m89j" target="_blank" title="Fale com o pastor.">Contactar</a></li>
                <li><a href="https://www.instagram.com/adtcgravier/" target="_blank" title="Instagram da igreja.">Instagram</a></li>
                <li><a href="mailto:rodrigollib3@gmail.com" target="_blank" title="Sugestões ao desenvolvedor.">Sugestões</a></li>
            </ul>
        </div>
        <div class="desenvolvedorSite">
            <small>Devolped By Rodrigo Liberato</small>
            <small>Copyright All Right Reserved 2025</small>
        </div>
    </footer>    
</template>

<script>

export default {
    name: 'rodapeSite' 
}


</script>

<style scoped>

footer {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 15vh;
    background-color: #252525;
    color:#ffff;

}

.linksrodape {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    width: 100%;
    height: 95px;
    padding: 15px;
    font-size: 14px;
}
.linksrodape ul {
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    list-style: none;
    width: 100%;
}
.linksrodape ul li {
    margin: 0 15px 0 15px;
}
.linksrodape a {
    text-decoration: none;
    color: #fff;
    font-weight: 300;
}

.desenvolvedorSite {
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: space-evenly;
    width: 85%;
    height: 15vh;
    padding: 15px;
    font-weight: 200;
    font-size: 15px;
    border-top: 1px solid #8b8b8b;
}
.desenvolvedorSite small {
    font-size: 8px;
}



</style>