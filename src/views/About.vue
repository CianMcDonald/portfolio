<template>
  <div class="about">
    <h1> About Me </h1>
    <div class="container">
      <aside>
        <ul>
          <h2> Skills </h2>
          <li>Python</li>
          <li>Java</li>
          <li>Vue</li>
          <li>React</li>
        </ul>
      </aside>
      <main>
        <h3> My name is Cian. I'm a third year computer science student based in Cork, Ireland.</h3>
        <p> I'm an avid learner and love nothing more than using new technologies.</p>
        <p> Outside of code I love sport and regularly take part in 5-aside soccer with an occasional Junior B hurling game too.</p>
      </main>
      </div>
    <figure>
      <figcaption>I also dabble in pumpkin art</figcaption>
      <img src="../assets/pumpkin.jpg" alt="pumpkin with small face">
      
    </figure>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>

  .about {
    text-align: center;
  }
  h1 {
    font-size: 3em;
  }
  h3 {
    font-size: 2em;
    font-weight: normal;
  }
  p {
    font-size:1.3em;
  }
  .container {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap-reverse;
  }
  main {
    text-align: left;
  }
  ul {
    text-align: left;
    font-size: 1.3em;
  }
  li {
    padding: 10px;
  }
  img {
      width:15%;
      min-width: 10%;
      border-radius: 10%;
  }
  figcaption {
    font-size: 1.2em;
  }
</style>