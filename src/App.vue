<template>
  <div id="app">
    <h3>El logo es parte del componente padre</h3>
    <img alt="Vue logo" src="./assets/logo.png">
    <GalleryComponent 
    title="Mi galeria" 
    :images_src="images"
    desc="Futbool">
     
      
      <p>Esto es parte del componenete padre</p>

    </GalleryComponent>
    
  </div>
</template>

<script>
import GalleryComponent from '@/components/GalleryComponent.vue';



export default {
  name: 'App',
  components: {
    GalleryComponent,
},
data:function(){
  return{
    images:[
  
 "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSxOPgtYb50ePdaLuGHkMlFLmBuUWtNeIqsKg&usqp=CAU",
 "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTtkU1G7ye4Vyy5uQnz_h8PtOdqu-Wc9M6kjg&usqp=CAU",
 "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS4MI0xQE8xRp1sawEucbBof8iFG_hgsA2WcQ&usqp=CAU"



    ],
  }
},

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
