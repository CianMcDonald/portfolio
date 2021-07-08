<template>
    <div class="container">
        <div>
        <h1> Hey, I'm Cian. </h1>
        <p> 
            Computer Science Student in University College Cork. <br>
            Vue, Python, Java Developer. <br>
            Excited to progress and learn more!
        </p>
        </div>
        <img src='../../assets/profile2.jpg'>
    </div>
</template>

<script>
export default {

}
</script>

<style scoped>
    img {
        width:15%;
        min-width: 10%;
        border-radius: 10%;
    }
    .container {
        padding-top: 1em;
        display: flex;
        justify-content: space-around;
        text-align: left;
        flex-wrap: wrap-reverse;
    }

    .container p {
        font-size: 2em;
    }
    h1 {
        font-size: 3em;
    }
</style>
