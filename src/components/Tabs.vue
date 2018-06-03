<template>
    <section class="container-fluid">
        <div class="row">
            <div class="col-md-12 pd">
                <h2>ELIGE TU VIAJE TRIP</h2>
            </div>
        </div>
        <div class="row">
            <div class="col-md-12">
                <br>
                <br>
                <ul class="nav nav-pills mb-3 justify-content-center" id="pills-tab" role="tablist">
                    <li class="nav-item">
                        <a class="nav-link active" id="pills-home-tab" data-toggle="pill" href="#pills-home" role="tab" aria-controls="pills-home" aria-selected="true">Basico</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" id="pills-profile-tab" data-toggle="pill" href="#pills-profile" role="tab" aria-controls="pills-profile" aria-selected="false">Premium</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" id="pills-contact-tab" data-toggle="pill" href="#pills-contact" role="tab" aria-controls="pills-contact" aria-selected="false">7 dias en la playa</a>
                    </li>
                </ul>
                <div class="tab-content" id="pills-tabContent">
                    <div class="tab-pane fade show active" id="pills-home" role="tabpanel" aria-labelledby="pills-home-tab">
                        <br>
                        <Pack 
                            title="Descubre tu destino sorpresa 2 días antes de viajar. Vuelo + hotel desde $200.000/pers."
                        
                        />
                    </div>
                    <div class="tab-pane fade" id="pills-profile" role="tabpanel" aria-labelledby="pills-profile-tab">
                        <br>
                        <Pack 
                            title="Escapada de 3 días por Latino America con hoteles premium y detalles exclusivos. Desde $350.000/pers."
                        />
                    </div>
                    <div class="tab-pane fade" id="pills-contact" role="tabpanel" aria-labelledby="pills-contact-tab">
                        <br>
                        <Pack 
                            title="Viaje sorpresa de 7 días en un destino de playa muy top. Vuelos + Hotel desde $500.000/pers."
                        />
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import Pack from './pack'
export default {
    components:{
        Pack
    }
}
</script>

<style scoped>
    section{
        min-height: 380px;
    }

    .nav-link{
        background: #fff;
        border:1px solid #eee;
        width: 300px;
        padding: 40px;
        border-radius: 0px;
        color: #22a6b3;
    }

    @media(max-width:991px){
        .nav-link{
            padding: 20px;
        }
    }

    .nav-link.active{
        border:2px solid #22a6b3;
        color: #fff;
        background: #22a6b3;
    }

    .pd{
        padding: 40px 40px 0px 40px;
    }
</style>
