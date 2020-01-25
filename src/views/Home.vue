


<template>
  <div class = "container-fluid text-center">
    <div class="row content">
      <div class="col-sm-2 sidenav">
        <p><a href="#">Link</a></p>
        <p><a href="#">Link</a></p>
        <p><a href="#">Link</a></p>
      </div>


    <div class="home container-fluid col-lg-8 text-left" >
      <div class= "row row-cols-4">
        <b-card v-for="club in clubs" :key="club"
          :title="club"
          img-src="https://picsum.photos/600/300/?image=25"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-2 col event-card"
        >
          <b-card-text>
          Some quick example text to build on the card title and make up the bulk of the card's content.
          </b-card-text>
          <b-button href="#" variant="primary">Go somewhere</b-button>
        </b-card>
    </div>
  
  </div>
   <div class="col-sm-2 sidenav">
      <div class="well">
        <p>ADS</p>
      </div>
      <div class="well">
        <p>ADS</p>
      </div>
    </div>
  </div>
  </div>
</template>
<style scoped>
body{
background-image: linear-gradient(to bottom, #051937, #171228, #190a1a, #12040d, #000000);
}
.event-card {
  margin: 10px;
  padding: 1rem;
}
</style>


<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'home',
  data()
  {
    return {
      clubs : ['MUSIC','club 2','club 3','club 4','club 2','club 4','club-7','club-8','club-9']
    }
  },

  components: {
    HelloWorld
  }
}
</script>
