<template>
<div>
    <div class="container-fluid">
        <div class="row mt-md-5 mt-sm-5 mt-xs-5">
            <div v-for="(art,indice) of datos" :key="art.id" class="col-lg-6 col-xs-12 border">
                <div v-if="indice<=3">
                <div  class="d-flex justify-content-center align-items-center">

                    <div class="p-3">
                        <svg width="12em" height="12em" viewBox="0 0 16 16" class="bi bi-alarm-fill" fill="currentColor" xmlns="http://www.w3.org/2000/svg">
                            <path fill-rule="evenodd" d="M6 .5a.5.5 0 0 1 .5-.5h3a.5.5 0 0 1 0 1H9v1.07a7.001 7.001 0 0 1 3.274 12.474l.601.602a.5.5 0 0 1-.707.708l-.746-.746A6.97 6.97 0 0 1 8 16a6.97 6.97 0 0 1-3.422-.892l-.746.746a.5.5 0 0 1-.707-.708l.602-.602A7.001 7.001 0 0 1 7 2.07V1h-.5A.5.5 0 0 1 6 .5zM.86 5.387A2.5 2.5 0 1 1 4.387 1.86 8.035 8.035 0 0 0 .86 5.387zM11.613 1.86a2.5 2.5 0 1 1 3.527 3.527 8.035 8.035 0 0 0-3.527-3.527zM8.5 5.5a.5.5 0 0 0-1 0v3.362l-1.429 2.38a.5.5 0 1 0 .858.515l1.5-2.5A.5.5 0 0 0 8.5 9V5.5z"
                            />
                        </svg>
                    </div>

                    <div class="p-2">
                        <p>
                            {{art.nombre}}
                        </p>
                    </div>

                </div>
                <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                    <button type="button" class="btn btn-outline-info">Info</button>
                </div>
                </div>
            </div>
        </div>
    </div>
    <div class="container">
        <div class="row justify-content-center mb-5">
            <div v-for="miembro in team" :key="miembro.codigo" class="col mt-5">
                     <div class="card text-white bg-dark" id='card'>
                        <div class="d-flex justify-content-center p-2">
                            <img :src="miembro.image" width="300" height="300">
                        </div>
                        <div class="card-body">
                            <h5 class="card-title">Empresa:</h5>
                            <h5 class="card-title"> {{miembro.nombre}}</h5>
                            <p class="card-text">{{miembro.descripcion}}
                            </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
    </div>
</template>


<script>
import axios from 'axios';
export default {
     data() {
        return {
            datos: null,
            team: [{
                
                nombre: 'Peter Szczesny/Papeles S.A.',
                descripcion: 'La empresa polaca con sede en colombia en cabeza del empresario Peter Szczesny realizó el proceso de administración de 3 informes, se identificaron pérdidas en tiempos de entrega del producto entre el área de producción y despacho y se logró una disminución en las pérdidas desde el 7% a solo el 3% de la producción.',
                image:"https://i.imgur.com/2hNPn6i.jpg"
            }, {
                
                nombre: 'Ferretería A MARTILLAR',
                descripcion: 'La ferretería logró ahorrarse más de 15 millones anuales en devoluciones después de efectuar un análisis de material invertido, se logró constatar que más de 20 millones anuales se perdían por falta de garantía de los proveedores a los artículos que se adquirían. ',
                image:"https://i.imgur.com/QoCIM0C.jpg"
            },  {
                
                nombre: ' Hilos e Hilos',
                descripcion: 'Hilos e Hilos con su nueva maquinaria que le ayuda a realizar 10 veces más rápido el trabajo en la confección de sus telas. El análisis nétamente productivo arrojó el atraso tecnológico en el área de producción. Hoy es una de las empresas con más tecnología en su sector.',
                image:" https://i.imgur.com/T7fMyZ2.jpg"
            }]
        };
    },
    mounted() {
     axios.get('articulo/list')
    .then(response => (this.datos = response.data));

    },
    
}
</script>
<style>
    #card{
        height: 720px;
        width: 350px;
    }
</style>