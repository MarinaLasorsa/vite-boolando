<script>
    export default {
        props: ['item']
    }
</script>

<template>
    <div class="card-header">
        <img :src="item.frontImage" alt="">
        <span class="heart-badge">&hearts;</span>
        <div>
            <span class="badge badge-green">Sostenibilità</span>
            <span class="badge badge-red">-50%</span>
        </div>
        <img :src="item.backImage" class="hover-image">
    </div>
    <div class="card-body">
        <p class="text-small">{{item.brand}}</p>
        <h5>{{item.name}}</h5>
        <p> <span class="text-small price">{{item.price}} &euro; </span><span class="text-small line-through">29,99 &euro;</span></p>
    </div>
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