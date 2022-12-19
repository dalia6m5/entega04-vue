<template>
    <div>
        
        <div class="row mb-4 d-flex justify-content-between align-items-center" v-for="(productocar, index) of productoscar" :key="index">
                            <div class="col-md-2 col-lg-2 col-xl-2">
                                 <img
                                    v-bind:src="productoscar[index].img"
                                    class="img-fluid rounded-3" :alt="productoscar[index].nombre">
                            </div>
                            <div class="col-md-3 col-lg-3 col-xl-3">
                                <h6 class="text-muted">{{productoscar[index].nombre}}</h6>
                                <h6 class="text-black mb-0">{{productoscar[index].marca}}</h6>
                            </div>
                           
                            <div class="col-md-3 col-lg-2 col-xl-2 offset-lg-1">
                            <h6 class="mb-0">${{productoscar[index].precio}}</h6>
                            </div>
                            <div class="col-md-1 col-lg-1 col-xl-1 text-end">
                            <a href="#!" class="text-muted"><i class="fas fa-times"></i></a>
                            </div>
        </div>

     
    </div>
  </template>
  
  <script>
  export default {
    name: 'ArticuloCarrito',
    props: {
        productoscar: Array
      
    }
  }
  </script>
  
  <style>
  
  </style>
  