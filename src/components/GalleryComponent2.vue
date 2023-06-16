<template>
    <div>
    <h1>{{ mensaje }}</h1>
    <button v-on:click="saludar">Saludo</button>
    <h2>{{ title }}</h2>
    <img v-bind:src="images_src" :alt="desc">
    
    



</div>
</template>

<script>
    export default{
        name: 'GalleryComponent',
        props: {
            title:{
                type:String,
                default:'El titulo por defecto'
            },
            images_src:{
                type: Array,
                required: true,

            },
            pepeito:{
                
            }
        }
        data: function(){
            return{
                mensaje: '',
            }
        },
        methods:{
            saludar: function(){
                this.mensaje='Este mensaje es parte del componente hijo';
            },
        }

    }



</script >


<style scoped>

div{
 border: 3px solid rgb(37,86,150);
 border-radius:10px;
 padding:10px;
 width:60%;
 margin:0 auto;
 background-color:rgb(58,136,226);
 color:white;
 }

 img{
 display:inline-block;
 border-radius:50%;
 margin-right: 10px;
 border:3px solid rgb(19,62,143);
 }





</style>