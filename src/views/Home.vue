<template>
  <div class="home">
    <Intro />
    <div class="projects">
      <h2> Projects </h2>
      <ul class="carousel">
        <li v-for="card in carousel" :key="card.id">
          <Card :heading="card.head" :text="card.text" :image='card.src' :description="card.description"/>
        </li>
      </ul>
    </div>
  </div>
   
</template>

<script>
// @ is an alias to /src
import Card from '../components/Card.vue'
import Intro from './Home/Intro.vue'

export default {
  name: 'Home',
  components: {
    Card, Intro
  },
  data() {
    return {
      carousel : [
        {id: 0, src:require('@/assets/logo.png'), head:'Website', text:"Douby", description:"Hella cool website",},
        {id: 1, src:require('@/assets/logo.png'), head:'App', text:"Scooby", description:"Hella cool website",},
        {id: 2, src:require('@/assets/logo.png'), head:'App', text:"Scooby", description:"Hella cool website",}
      ],
    }
  }
}
</script>

<style scoped>
  .projects {
    padding-top: 3em;
    font-size: 1.2em;;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .carousel {
    padding-top: 2em;
    list-style-type: none;
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    padding-left: 0;
  }


</style>
