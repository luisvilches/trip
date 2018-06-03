<template>
    <div class="card">
        <img src="../assets/basic.jpg" class="img-fluid" alt="">
        <div class="body">
            <br>
            <h5>Trip {{data.type}}</h5>
            <h6>desde ${{data.price}}/pers.</h6>
            <table>
                <tbody class="text-left">
                    <tr class="border">
                        <p><i class="fas fa-sun space"></i> {{data.days}} </p>
                    </tr>
                    <tr class="border">
                        <p><i class="fas fa-map-marker-alt space"></i> {{data.info}}</p>
                    </tr>
                    <tr class="border">
                       <p><i class="fas fa-plane space"></i> {{data.ida}}</p>
                    </tr>
                    <tr class="border">
                        <p><i class="fas fa-h-square space"></i> {{data.hotel}} <i class="fas fa-star"></i></p>
                    </tr>
                    <tr>
                        <p><i class="fas fa-coffee space"></i> {{data.desayuno}}</p>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>

<script>
export default {
    props:[
        'data'
    ]
}
</script>

<style scoped>
    .card{
        box-shadow: 0px 0px 5px #eee;
        border-radius: 20px;
        margin-bottom: 40px;
    }
    .body{
        border-radius: 20px;
    }
    img{
        border-radius: 20px 20px 0px 0px;
    }
    .border{
        border-bottom: 1px solid #ccc;
    }
    table{
        width: 100%;
    }
    p{
        padding:20px 20px 0px 20px;
        margin-left: 20px;
    }
    .fa-star{
        font-size: 10px;
        position: relative;
        top: -1px;
    }

    .space{
        margin-right: 20px;
    }
</style>
