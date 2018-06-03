<template>
    <section>
        <div class="overlay"></div>
        <div class="container">
            <div class="row">
                <div class="col-md-12 text-center">
                    <h2>¿Como funciona Trip?</h2>
                </div>
            </div>
            <div class="row">
                <div class="col-md-4">
                    <img src="../assets/wall-calendar.png" alt="">
                    <h4>CONFIGURA TU VIAJE</h4>
                    <p>Elige el tipo de viaje sorpresa que más se ajusta a ti. Indica el número de viajeros, el aeropuerto de origen y las fechas en las que quieres viajar.</p>
                </div>
                <div class="col-md-4">
                    <img src="../assets/placeholder.png" alt="">
                    <h4>ELIMINA DESTINOS</h4>
                    <p>Descubre tus 12 destinos posibles. ¿Le tienes manía a alguno? Elimina las ciudades que NO quieres visitar</p>
                </div>
                <div class="col-md-4">
                    <img src="../assets/gift.png" alt="">
                    <h4>¡SORPRESA!</h4>
                    <p>Dos días antes de volar, te desvelaremos tu destino, vuelos y alojamiento y te entregaremos una guía exclusiva de tu viaje</p>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    
}
</script>

<style scoped>
    section{
        background-attachment: fixed;
        background-image: url('.././assets/section2.jpg');
        width: 100%;
        min-height: 600px;
        background-repeat: no-repeat;
        position: relative;
    }

    .overlay{
        background-color: #222534;
        position: absolute;
        top: 0;
        left: 0;
        display: block;
        width: 100%;
        height: 100%;
        opacity: 0.6;
        filter: alpha(opacity=40);
        z-index: 0;
    }

    h2{
        margin-top:80px;
        color:#fff;
        font-size: 40px;
    }

    img{
        max-width: 100px;
        margin-top:100px;
        margin-bottom: 40px;
    }
    h4{
        color: #fff;
        margin-bottom: 20px;
    }
    p{
        color: #fff;
        letter-spacing: 1.5px;
    }
</style>
