<script setup>
    import logoimg from '../assets/logo.png'
</script>
<template>
    <header class="main-header">
        <div class="logo-container">
            <a href="#inicio">
                <img :src="logoimg" alt="logo"/>
            </a>
        </div>

        <nav class="nav-links">
            <a href="#nosotros">Nosotros</a>
            <a href="#que-hacemos">Que hacemos</a>
            <a href="#por-que-contratarnos">Por que contratarnos</a>
            <a href="#contacto">Contacto</a>
        </nav>

    </header>
</template>

<style scoped>
        .main-header{
            display: flex;
            position:fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            justify-content: space-between;
            align-items: center;
            background-color: #f7f6f2;
            padding: 15px 60px;
        }

        .logo-container img {
            height: 50px;
            width: auto;
        }

        .nav-links a {
            text-decoration: none;
            color: black;
            font-weight: bold;
            margin: 0 20px;
            outline: none;
            background: none;
            box-shadow: none;
        }

        .nav-links a:hover {
            color:#6b6b6b;
        }

        .nav-links a {
            color:black;
        }

        .nav-links a:last-child {
            background-color: #b5ff5d;
            padding: 10px 20px;
            border-radius: 20px;
        }

        .nav-links a:last-child:hover{
            background-color: #9de64f;
            transform: scale(1.05);
            transition: 0.2s;
        }
</style>