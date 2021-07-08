<template>
     <div class="flip-card">
        <div class="flip-card-inner">
            <div class="flip-card-front">
                <img :src= 'image' alt="Avatar" >
                <h3><b>{{heading}}</b></h3>
                <p>{{text}}</p>
            </div>
            <div class="flip-card-back">
                <h1> {{heading}} </h1>
                <p> {{description}} </p>
            </div>
        </div>
    </div>  
</template>

<script>
export default {
    props: ['image', 'heading', 'text', 'description',]
}
</script>

<style>
    img {
        max-width: 100%;
    }
    
    .flip-card {
        /* Add shadows to create the "card" effect */
        border: 1px solid #f1f1f1;
        border-radius: 10%;
        background-color: transparent;
        width: 16em;
        height: 23em;
        perspective: 1000px;
    }

    .flip-card-inner {
        position: relative;
        width: 100%;
        height: 100%;
        text-align: center;
        transition: transform 0.8s;
        transform-style: preserve-3d;
    }

    /* horizontal flip on hover */
    .flip-card:hover .flip-card-inner {
        transform: rotateY(180deg);
    }

    .flip-card-front, .flip-card-back {
        position: absolute;
        width: 100%;
        height: 100%;
        -webkit-backface-visibility: hidden; /* Safari */
        backface-visibility: hidden;
        border-radius: 10%;
    }

    .flip-card-front {
        font-size: 1.2em;
    }

    .flip-card-back {
        background-color: #363537;
        color: white;
        transform: rotateY(180deg);
    }
</style>