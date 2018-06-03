<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-md-12">
                    <h3 class="title">{{title}}</h3>
                </div>
            </div>
            <div class="row">
                <div class="col-md-3">
                    <label for="">¿Para quien?</label>
                    <v-select v-model="para" :options="['Mi','Regalar']"></v-select>
                </div>
                <div class="col-md-3">
                    <label for="">¿Cuantos somos?</label>
                    <v-select v-model="cantidad" :options="cuantos"></v-select>
                </div>
                <div class="col-md-3">
                    <label for="">¿Desde donde?</label>
                    <v-select v-model="donde" :options="['foo','bar']"></v-select>
                </div>
                <div class="col-md-3">
                    <label for="">Reservar</label>
                    <button @click="send" class="btn-reservar form-control">Comenzar</button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data(){
        return {
            cuantos:[],
            cantidad:"",
            para:"",
            donde:""
        }
    },
    created(){
        var index = 1;
        while(index <= 10){
            this.cuantos.push(String(index));
            index++;
        }
    },
    components:{
    
    },
    props:[
        'title',
    ],
    methods:{
        send(){
            console.log(this.cantidad,this.para,this.donde);
        }
    }
}
</script>

<style scoped>
    .container{
        border-radius: 5px;
        border: 1px solid #c1c1c1;
        min-height: 300px;
        padding: 20px;
    }

    h3.title{
        margin-bottom: 60px;
        margin-top: 20px;
        color: #333;
    }

    .btn-reservar{
        background: #dc3545;
        border-color: #dc3545;
        color: #fff;
        border:none;
        cursor: pointer;
        outline: 0;
    }

    @media(max-width:991px){
        .btn-reservar{
            padding: 20px;
        }

        section{
            margin-bottom: 40px;
        }
    }

    .btn-reservar:hover{
        background-color: #c82333;
        border-color: #bd2130;
    }

    .btn-reservar:focus,.btn-reservar:active{
        outline: 0;
        border:none;
        box-shadow: none;
    }
</style>
