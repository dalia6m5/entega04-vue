<template>
    <div>
         <section class="vh-100 gradient-custom">
            <div class="container py-5 h-100">
                <div class="row d-flex justify-content-center align-items-center h-100 " >
                    <div class="col-12 col-md-8 col-lg-6 col-xl-5 border border-secondary p-4 m-4" style="border-radius: 1rem;" >
                        <h5>Productos disponibles</h5>
                        <div class="card bg-secondary text-white" style="border-radius: 1rem;">
                        
                        <TarjetaProducto :productoslista="productoslista"/>
                        
                        </div>

                    </div>
                </div>
            </div>
         </section>
     
    </div>
  </template>
  
  <script>

import TarjetaProducto from './TarjetaProducto.vue';

  export default {
    name: 'ListaProd',
    components: { 
        TarjetaProducto 
    },
    data:function (){
        return{
            productoslista:[
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
                img: require("../assets/Foto-02.jpg"),
                descripcion:"Retinol estabilizado RetiStar al 1 % y retinoide granactivo al 0,5 %: reduce la apariencia de las líneas finas y las arrugas; fórmula de liberación lenta para una entrega activa eficaz y poco irritante. Escualano: Hidrata y calma."
            },
            {
                id:3,
                nombre:"Retinol 0.3%",
                marca: "Cerave",
                precio: 13,
                img: require("../assets/Foto-03.jpg"),
                descripcion:"Un sérum de tratamiento post-imperfecciones con retinol encapsulado, extracto de raíz de regaliz y niacinamida que ayuda a que la piel tenga un aspecto más brillante, suave y uniforme."
            },
            {
                id:4,
                nombre:"Reti-Age",
                marca: "Sesderma",
                precio: 9,
                img: require("../assets/Foto-04.jpg"),
                descripcion:"Potente acción antienvejecimiento y excelente tolerancia gracias a su Sistema 3-Retinol de liberación sostenida. Los retinoides estimulan la proliferación de los queratinocitos, normalizan el proceso de exfoliación, mejoran la textura y tono de la piel. "
            },
            {
                id:5,
                nombre:"Retinol B3",
                marca: "Roche Posay",
                precio: 23,
                img: require("../assets/Foto-05.jpg"),
                descripcion:"El serum facial Retinol B3 La Roche-Posay te ayuda con la regeneración y cuidado de la piel. Su fórmula anti-arrugas con vitamina B3 es ideal para el tratamiento de arrugas profundas, tono irregular y fotoenvejecimiento."

            },
            
        ],
        }
        
    }
  }
  </script>
  
  <style>
  
  </style>