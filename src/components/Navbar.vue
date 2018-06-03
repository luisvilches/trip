<template>
    <nav class="navbar navbar-expand-lg fixed-top">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
            <span class="fas fa-bars"></span>
        </button>
        <router-link to="" class="logo mobile">trip</router-link>
        <li class="nav-item mobile">
            <router-link to="" ><i class="fas fa-gift"></i></router-link>
        </li>
        <li class="nav-item circle mobile">
            <router-link to="" ><i class="fas fa-user"></i></router-link>
        </li>
        <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
            <router-link to="" class="logo desktop">trip</router-link>
            <ul class="navbar-nav ml-auto mt-2 mt-lg-0">
                <li class="nav-item active">
                    <router-link to="" >CÓMO FUNCIONA</router-link>
                </li>
                <li class="nav-item">
                    <router-link to="" >HOTELES</router-link>
                </li>
                <li class="nav-item">
                    <router-link to="" >AYUDA</router-link>
                </li>
                <li class="nav-item">
                    <router-link to="" >CONTACTO</router-link>
                </li>
                <li class="nav-item desktop red">
                    <router-link to="" ><i class="fas fa-gift"></i> ¡REGALA TRIP!</router-link>
                </li>
                <li class="nav-item desktop red bg-red">
                    <router-link to="" >RESERVAR</router-link>
                </li>
            </ul>
        </div>
    </nav>
</template>

<script>
export default {
    created(){},
    mounted(){}
}
</script>

<style scoped>

    nav{
        background:#fff;
        border-bottom: 1px solid #eee;
        padding: 15px 20px 15px 20px;
        box-shadow: 0px 0px 3px #eee;
    }
    .logo{
        font-family: 'Comfortaa', cursive !important;
        font-size: 40px;
        margin-left: 30px;
        color: #22a6b3;
    }
    ul li{
        list-style: none;
        display: inline-block;
        margin: 0px 5px;
        padding: 10px 20px;
    }
    ul li a{
        font-size: 14px;
        text-decoration: none;
        color: #22a6b3;
    }
    ul li:hover{
        /*background: #22a6b3;
        border-radius: 5px;*/
        cursor: pointer;
    }

    ul li:hover a{
        color: #bd2130;
    }

    .logo:hover{background:#fff;}
    .logo:hover a{color: #22a6b3;}

    .circle{
        border:2px solid #22a6b3;
        border-radius: 100%!important;
    }

    .nav-item a{
        color: #22a6b3;
    }

    .nav-item{
        border: none;
    }

    .red a{
        color: #dc3545;
    }

    .bg-red{
        background: #dc3545;
        border-color: #dc3545;
        border-radius: 5px;
        
    }
    .bg-red a {
        color:#fff!important;
    }

    .bg-red:hover{
        background-color: #c82333;
        border-color: #bd2130;
        border-radius: 5px;  
    }

    @media (min-width: 991px){
        .desktop{
            display: block;
        }
        .mobile{
            display: none;
        }
    }

    @media (max-width: 990px){
        .desktop{
            display: none;
        }
        .mobile{
            display: block;
        }

        .navbar-nav li {
            text-align: left;
        }

        .circle{
            max-width: 35px;
        }
    }
</style>
