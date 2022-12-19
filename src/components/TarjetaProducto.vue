<template>
    <div>
        <section v-for="(productolista, index) of productoslista" :key="index">
        <div class="card tarjeta m-4" style="width: 18rem;">
            <img :src="productoslista[index].img" class="card-img-top" :alt="productoslista[index].nombre">
            <div class="card-body text-secondary">
                <h5 class="card-title">{{productoslista[index].nombre}}</h5>
                <p class="card-text">$ {{productoslista[index].precio}}</p>
                <a href="#" class="btn btn-primary">Agregar al carrito</a>
            </div>
        </div>
     </section>
    </div>
  </template>
  
  <script>
  export default {
    name: 'TarjetaProducto',
    props: {
        productoslista: Array
      
    }
  }
  </script>
  
  <style>

  
  </style>
  