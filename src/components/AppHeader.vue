<script>
</script>

<template>
    <header class="page-header">
        <nav class="container">
            <div class="row"> 
                <ul class="link-menu">
                    <li><a href="#">Donna</a></li>
                    <li><a href="#">Uomo</a></li>
                    <li><a href="#">Bambini</a></li>
                </ul>
                <div class="logo">
                    <img src="/boolean-logo.png">
                </div>
                <ul class="link-menu">
                    <li>buttons</li>
                </ul>
            </div>
        </nav>
    </header>
</template>

<style scoped>
    .page-header {
        background-color: rgb(255, 102, 0);
        padding: 10px 0;
        color: white;
        font-size: 14px;
        position: fixed;
        width: 100%;
        z-index: 1000;
    }

    .page-header .row {
        align-items: center;
        gap: 20px;
    }

    .logo img {
        height: 22px;
    }

    .link-menu {
        display: flex;
        align-items: center;
        gap: 10px;
        font-weight: bold;
    }
</style>