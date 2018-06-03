<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-md-12 pd">
                    <h2>DESCUBRE TODOS LOS VIAJES TRIP</h2>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4">
                    <Card :data="basico"/>
                </div>
                <div class="col-md-4">
                    <Card :data="premium"/>
                </div>
                <div class="col-md-4">
                    <Card :data="playa"/>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Card from './card'
export default {
    components:{
        Card
    },
    data(){
        return {
            basico:{
                type:'Basico',
                price:'200.000',
                img:'../assets/basic.jpg',
                days:'Viaje de 3 ó 5 días',
                info:' 1 destino sorpresa',
                ida:' Vuelos directos de ida y vuelta',
                hotel:'Alojamiento céntrico 3/5',
                desayuno:' No incluye el desayuno'
            },
            premium:{
                type:'Premium',
                price:'350.000',
                img:'../assets/basic.jpg',
                days:' Viaje de 3 días (2 noches)',
                info:'1 destino sorpresa',
                ida:' Vuelos directos de ida y vuelta',
                hotel:' Alojamiento céntrico 3/5',
                desayuno:'Desayuno incluido!'
            },
            playa:{
                type:'7 dias en la playa',
                price:'500.000',
                img:'../assets/basic.jpg',
                days:' Viaje de 7 días (6 noches)',
                info:'1 destino sorpresa',
                ida:'Vuelos directos de ida y vuelta',
                hotel:'Alojamiento céntrico 3/5',
                desayuno:' No incluye el desayuno'
            }
        }
    }
}
</script>

<style scoped>
    section{
        padding: 20px;
        min-height: 400px;
    }

    .pd{
        padding: 40px;
    }

    @media(max-width:991px){
        .pd{
            padding: 40px 20px;
        }
    }
</style>
