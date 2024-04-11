<script>
    import AppCard from './AppCard.vue'

    export default {
        components: {
            AppCard
        },
        data () {
            return {
                products: [
                    {
                    "id": 1,
                    "frontImage": "1.webp",
                    "backImage": "1b.webp",
                    "brand": "Levi's",
                    "name": "Relaxed Fit",
                    "price": 29.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                        "type": "tag",
                        "value": "Sostenibilità"
                        },
                        {
                        "type": "discount",
                        "value": "-50%"
                        }
                    ]
                    },
                    {
                    "id": 2,
                    "frontImage": "2.webp",
                    "backImage": "2b.webp",
                    "brand": "Guess",
                    "name": "Roses Tee",
                    "price": 20.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                        "type": "discount",
                        "value": "-30%"
                        }
                    ]
                    },
                    {
                    "id": 3,
                    "frontImage": "3.webp",
                    "backImage": "3b.webp",
                    "brand": "Come Zucchero Filato",
                    "name": "Voglia di colori pastello",
                    "price": 129.99,
                    "isInFavorites": false,
                    "badges": [
                        {
                        "type": "discount",
                        "value": "-30%"
                        }
                    ]
                    },
                    {
                    "id": 4,
                    "frontImage": "4.webp",
                    "backImage": "4b.webp",
                    "brand": "Levi's",
                    "name": "Tee Unisex",
                    "price": 14.99,
                    "isInFavorites": false,
                    "badges": [
                        {
                        "type": "tag",
                        "value": "Sostenibilità"
                        },
                        {
                        "type": "discount",
                        "value": "-50%"
                        }
                    ]
                    },
                    {
                    "id": 5,
                    "frontImage": "5.webp",
                    "backImage": "5b.webp",
                    "brand": "Maya Deluxe",
                    "name": "Stripe Bodice",
                    "price": 99.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                        "type": "tag",
                        "value": "Sostenibilità"
                        },
                        {
                        "type": "discount",
                        "value": "-50%"
                        }
                    ]
                    },
                    {
                    "id": 6,
                    "frontImage": "6.webp",
                    "backImage": "6b.webp",
                    "brand": "Esprit",
                    "name": "Maglione - Black",
                    "price": 29.99,
                    "isInFavorites": true,
                    "badges": [
                        {
                        "type": "tag",
                        "value": "Sostenibilità"
                        }
                    ]
                    }
                ]
            }
        }
    }
</script>

<template>
    <main class="page-content">
        <div class="container"> 
            <div class="row"> 
                <AppCard v-for="(card, i) in products" :item="card" :key="i"/>
                <!--<div class="col-1-3">
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
                </div>-->
            </div>
        </div>
    </main>
</template>

<style scoped>

    
</style>