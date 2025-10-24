<script setup>
import Header from './components/Header.vue';
import arrowLeft from './assets/iconleft.png';
import arrowRight from './assets/iconright.png';
</script>

<template>
<Header/>

<main class="main-content">
    
    <section id="nosotros" class="section">
        <div class="right">
            <img :src="arrowLeft" alt="iconleft"/>
            <h2>Nosotros</h2>
        </div>
    </section>

    <section id="que-hacemos" class="section">
        <div class="left">
            <h2>Que hacemos</h2>
            <img :src="arrowRight" alt="iconright"/>
        </div>
        </section>

    <section id="por-que-contratarnos" class="section">
        <div class="right">
            <img :src="arrowLeft" alt="iconleft"/>
            <h2>Porque contratarnos</h2>
        </div>
    </section>

    <section id="contacto" class="section">
        <div class="left">
            <h2>Contacto</h2>
            <img :src="arrowRight" alt="iconright"/>
        </div>
    </section>
    


</main>

</template>

<style scoped>
    .main-content {
        margin-top: 80px;
    }

    .section {
        position: relative;
        min-height: 100vh;
        color: black;  
        scroll-margin-top: 85px;
    }

    #nosotros, #por-que-contratarnos  {
        background-color: whitesmoke;
    }

    #contacto, #que-hacemos {
        background-color: greenyellow;
    }

    .right {
        display: flex;
        justify-content: right;
        padding: 30px;
        align-items: center;
    }

    .left {
        display: flex;
        justify-content: left;
        padding: 30px;
        align-items: center;
    }


    .left img, .right img {
        width: 29px;
        height: 29px;
        margin: 12px;
    }

</style>
