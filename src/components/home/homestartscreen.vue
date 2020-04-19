<template>
    <div class="container-fluid">
        <div class="row py-5 align-items-center">
            <div class="col-md-4 text-center">
                <img class="profileimg" :src="maindata1.imgUrl" alt="">
            </div>
            <div class="col-md-8">
                <h1>{{maindata1.name}}</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta animi corporis, veritatis</p>
                <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta animi corporis, veritatis</p>
                <button class="btn btn-primary">Hire me</button>
            </div>
        </div>
    </div>
</template>
<script>
import maindata from '@/assets/data/main.json'
    export default {
        name:'HomeScreen',
        data:()=>({
            maindata1:maindata
        })
    }
</script>

<style>
    .profileimg{
        border-radius: 50%;
        width: 80%;
        margin-left: auto;
        margin-right: auto;
    }
</style>