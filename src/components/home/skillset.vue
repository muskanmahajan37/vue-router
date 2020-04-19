<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-md-4">
                <h1>Skils</h1>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Asperiores facere optio earum quaerat, quos aliquid quia? Commodi tempora earum nam, fugiat rem animi provident delectus possimus quo, neque sunt id.</p>
            </div>
            <div class="col-md-8">
                <div class="container-fluid">
                    <div class="row">
                        <div class="col-md-3 m-1" v-for="(item,index) in mainData1.skills" :key="index">
                            <div class="card py-2 px-3">
                                {{item}}
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import maindata from '@/assets/data/main.json'
    export default {
        name:'Skillsets',
        data:()=>({
            mainData1: maindata
        }),
        methods:{

        }
    }
</script>

<style>
    .skills{
        
        border: 1px solid black;
        border-radius: 5px;
    }
    .skills:hover{
        background-color: black;
        color: white;
    }
</style>