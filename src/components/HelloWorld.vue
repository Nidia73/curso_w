<template>
  <div>
    <div>
      <h1>Contenido</h1>
    </div>
  </div>
 </template> 

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return {
      nombre : 'Nidia',
      mostrar : true,
      clientes :[{id:1,nombre : 'Nidia'},{id:2,nombre:'Margoth'}],
      url : 'https://www.google.com',
      numero1 :0,
      numero2 :0,
      resultado :0,
      tarea : null,
      tareas : []
    }
  },
  methods :{
    metodo1(){
      alert("Click")
     /*console.log('Ingrese el metodo')*/
    },
    sumar(){
      this.resultado= this.numero1 + this.numero2
    },
    restar(){
      this.resultado= this.numero1 - this.numero2
    },
    multiplicar(){
      this.resultado= this.numero1 * this.numero2
    },
    dividir(){
      this.resultado= this.numero1 / this.numero2
    },
    agregarTarea(){
      alert("Agregar tarea"+this.tarea)
      this.tareas.push(this.tarea)
    }
  }
}
</script>


<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  color:blue;
  font-size: 34px;
}
a {
  color: #42b983;
}
</style>
