<template>
    <div>
        <section class="h-100 h-custom" style="background-color: #d2c9ff;">
        <div class="container py-5 h-100">
            <div class="row d-flex justify-content-center align-items-center h-100">
            <div class="col-12">
                <div class="card card-registration card-registration-2" style="border-radius: 15px;">
                <div class="card-body p-0">
                    <div class="row g-0">
                    <div class="col-lg-8">
                        <div class="p-5">
                        <div class="d-flex justify-content-between align-items-center mb-5">
                            <h1 class="fw-bold mb-0 text-black">Carrito</h1>
                            <h6 class="mb-0 text-muted">3 productos</h6>
                        </div>
                        <hr class="my-4">

                      <articulo-carrito :productoscar="productoscar"/>

                        <hr class="my-4">


                        <div class="pt-5">
                            <h6 class="mb-0"><a href="#!" class="text-body"><i
                                class="fas fa-long-arrow-alt-left me-2"></i>Seguir comprando</a></h6>
                        </div>
                        </div>
                    </div>
                    <!-- <div class="col-lg-4 bg-grey">
                        <div class="p-5">
                        <h3 class="fw-bold mb-5 mt-2 pt-1">Summary</h3>
                        <hr class="my-4">

                        <div class="d-flex justify-content-between mb-4">
                            <h5 class="text-uppercase">items 3</h5>
                            <h5>€ 132.00</h5>
                        </div>

                        <h5 class="text-uppercase mb-3">Shipping</h5>

                        <div class="mb-4 pb-2">
                            <select class="select">
                            <option value="1">Standard-Delivery- €5.00</option>
                            <option value="2">Two</option>
                            <option value="3">Three</option>
                            <option value="4">Four</option>
                            </select>
                        </div>

                        <h5 class="text-uppercase mb-3">Give code</h5>

                        <div class="mb-5">
                            <div class="form-outline">
                            <input type="text" id="form3Examplea2" class="form-control form-control-lg" />
                            <label class="form-label" for="form3Examplea2">Enter your code</label>
                            </div>
                        </div>

                        <hr class="my-4">

                        <div class="d-flex justify-content-between mb-5">
                            <h5 class="text-uppercase">Total price</h5>
                            <h5>€ 137.00</h5>
                        </div>

                        <button type="button" class="btn btn-dark btn-block btn-lg"
                            data-mdb-ripple-color="dark">Register</button>

                        </div>
                    </div> -->
                    </div>
                </div>
                </div>
            </div>
            </div>
        </div>
        </section>
    </div>
  </template>
  
  <script>
import ArticuloCarrito from './ArticuloCarrito.vue';

  export default {
    name: "TarjetaProducto",
   
    components: { 
        ArticuloCarrito 
    },
    data:function (){
        return{
            productoscar:[
            {
                id:1,
                nombre:"Retinol 1%",
                marca: "Paulas Choice",
                precio: 30,
                img: require("../assets/Foto-01.jpg"),
                descripcion:"Paula's Choice El tratamiento clínico de retinol al 1% con péptidos y vitamina C está formulado para reducir la apariencia de arrugas, ya que refina los poros y reafirma la piel para una apariencia radiante, rejuvenecida y juvenil. Esta fórmula robusta también ayuda a prevenir signos de envejecimiento y suaviza el aspecto de las marcas postacné."
            },
            {
                id:2,
                nombre:"Retinol 0.3%",
                marca: "Inkey List",
                precio: 10,
                img: require("../assets/Foto-04.jpg"),
                descripcion:"Retinol estabilizado RetiStar al 1 % y retinoide granactivo al 0,5 %: reduce la apariencia de las líneas finas y las arrugas; fórmula de liberación lenta para una entrega activa eficaz y poco irritante. Escualano: Hidrata y calma."
            },
            {
                id:3,
                nombre:"Retinol 0.3%",
                marca: "Cerave",
                precio: 13,
                img: require("../assets/Foto-02.jpg"),
                descripcion:"Un sérum de tratamiento post-imperfecciones con retinol encapsulado, extracto de raíz de regaliz y niacinamida que ayuda a que la piel tenga un aspecto más brillante, suave y uniforme."
            },
            
        ],
        }
        
    }
}
  </script>
  
  <style>
  
  </style>
  