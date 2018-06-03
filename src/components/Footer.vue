<template>
    <footer>
        <div class="container text-left">
            <div class="row">
                <div class="col-md-3">
                    <h6>MENÚ PRINCIPAL</h6>
                    <ul>
                        <li><router-link to="">Como funciona</router-link></li>
                        <li><router-link to="">Hoteles</router-link></li>
                        <li><router-link to="">Ayuda</router-link></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h6>MÁS INFORMACIÓN</h6>
                    <ul>
                        <li><router-link to="">Quines somos</router-link></li>
                        <li><router-link to="">Trabaja con nosotros</router-link></li>
                        <li><router-link to="">Blog</router-link></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h6>CONTÁCTANOS</h6>
                    <ul class="info left">
                        <li><router-link to=""><i class="fas fa-envelope-open"></i> hola@trip.cl</router-link></li>
                        <li><router-link to=""><i class="fas fa-phone"></i> +56 2 2233 1234</router-link></li>
                        <li><router-link to=""><i class="fas fa-mobile-alt"></i> +56 9 8492 3552</router-link></li>
                    </ul>
                </div>
                <div class="col-md-3">
                    <h6>SÍGUENOS EN</h6>
                    <ul class="rrss left">
                        <li><router-link to=""><i class="fab fa-facebook-square"></i></router-link></li>
                        <li><router-link to=""><i class="fab fa-twitter-square"></i></router-link></li>
                        <li><router-link to=""><i class="fab fa-instagram"></i></router-link></li>
                        <li><router-link to=""><i class="fab fa-youtube"></i></router-link></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    
}
</script>

<style scoped>

    footer{
        background: #222534;
        padding:80px;
        height: 300px;
    }

    .left{
        margin-left: 10px;
    }
    ul li{
        list-style: none;
        margin-bottom: 20px;
    }

    ul li a{
        color: #fff;
    }

    .rrss li{
        display: inline-block;
        margin-right: 10px;
    }

    .rrss li a{
        font-size: 30px;
    }

    h6{
        text-align: center;
        font-size: 23px;
        color:#fff;
        margin-bottom: 20px;
    }

    .info i{
        margin-right: 10px;
    }
</style>
