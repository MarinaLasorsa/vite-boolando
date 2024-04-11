<script>
</script>

<template>
    <main class="page-content">
        <div class="container"> 
            <div class="row"> 
                <div class="col-1-3">
                    <div class="card-header">
                        <img src="/1.webp" alt="">
                        <span class="heart-badge">&hearts;</span>
                        <div>
                            <span class="badge badge-green">Sostenibilità</span>
                            <span class="badge badge-red">-50%</span>
                        </div>
                        <img src="/1b.webp" class="hover-image">
                    </div>
                    <div class="card-body">
                        <p class="text-small">Levi's</p>
                        <h5>RELAXED FIT TEE UNISEX</h5>
                        <p> <span class="text-small price">14,99 &euro; </span><span class="text-small line-through">29,99 &euro;</span></p>
                    </div>
                </div>
                <div class="col-1-3">
                    <div class="card-header">
                        <img src="/2.webp" alt="">
                        <span class="heart-badge">&hearts;</span>
                        <div>
                            <span class="badge badge-red">-30%</span>
                        </div>
                        <img src="/2b.webp" class="hover-image">
                    </div>
                    <div class="card-body">
                        <p class="text-small">Guess</p>
                        <h5>ROSES TEE</h5>
                        <p> <span class="text-small price">20,99 &euro; </span><span class="text-small line-through">29,99 &euro;</span></p>
                    </div>
                </div>
                <div class="col-1-3">
                    <div class="card-header">
                        <img src="/3.webp" alt="">
                        <span class="heart-badge">&hearts;</span>
                        <div>
                            <span class="badge badge-red">-30%</span>
                        </div>
                        <img src="/3b.webp" class="hover-image">
                    </div>
                    <div class="card-body">
                        <p class="text-small">Come Zucchero Filato</p>
                        <h5>VOGLIA DI COLORI PASTELLO</h5>
                        <p> <span class="text-small price">129,99 &euro; </span><span class="text-small line-through">184,99 &euro;</span></p>
                    </div>
                </div>
                <div class="col-1-3">
                    <div class="card-header">
                        <img src="/4.webp" alt="">
                        <span class="heart-badge">&hearts;</span>
                        <div>
                            <span class="badge badge-green">Sostenibilità</span>
                            <span class="badge badge-red">-50%</span>
                        </div>
                        <img src="/4b.webp" class="hover-image">
                    </div>
                    <div class="card-body">
                        <p class="text-small">Levi's</p>
                        <h5>TEE UNISEX</h5>
                        <p> <span class="text-small price">14,99 &euro; </span><span class="text-small line-through">29,99 &euro;</span></p>
                    </div>
                </div>
                <div class="col-1-3">
                    <div class="card-header">
                        <img src="/5.webp" alt="">
                        <span class="heart-badge">&hearts;</span>
                        <img src="/5b.webp" class="hover-image">
                    </div>
                    <div class="card-body">
                        <p class="text-small">Maya Deluxe</p>
                        <h5>STRIPE BODICE</h5>
                        <p> <span class="text-small price">99,99 &euro; </span><span class="text-small line-through">29,99 &euro;</span></p>
                    </div>
                </div>
                <div class="col-1-3">
                    <div class="card-header">
                        <img src="/6.webp" alt="">
                        <span class="heart-badge">&hearts;</span>
                        <div class="not-on-sale">
                            <span class="badge badge-green">Sostenibilità</span>
                        </div>
                        <img src="/6b.webp" class="hover-image">
                    </div>
                    <div class="card-body">
                        <p class="text-small">Esprit</p>
                        <h5>MAGLIONE - BLACK</h5>
                        <p> <span class="text-small price">29,99 &euro; </span></p>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style scoped>

    /*CARD*/

    .card-header {
        position: relative;
    }

    .card-body .text-small {
        font-size: 12px;
    }

    .price {
        font-weight: bold;
        color: red;
    }

    .hover-image {
        position: absolute;
        top: 0;
        left: 0;
        opacity: 0
    }

    .col-1-3:hover .hover-image {
        opacity: 1
    }

    /*COMPONENTS*/

    .heart-badge {
        background-color: rgb(255, 255, 255);
        font-size: 30px;
        padding: 0 10px;
        position: absolute;
        right: 0;
        top: 10px;
        z-index: 999;
    }

    .badge {
        color: white;
        font-size: 10px;
        padding: 5px;
        font-weight: bold;
        z-index: 999;

    }

    .badge.badge-green {
        background-color: green;
        position: absolute;
        left: 35px;
        bottom: 35px;
    }

    .badge.badge-red {
        background-color: red;
        position: absolute;
        left: 0;
        bottom: 35px;
    }

    .not-on-sale .badge.badge-green {
        position: absolute;
        left: 0px;
        bottom: 35px;
    }
</style>