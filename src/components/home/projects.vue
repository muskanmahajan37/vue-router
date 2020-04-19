<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-md-12 text-center py-2">
                <h1>Projects</h1>
            </div>
        </div>
        <div class="row">
            <div class="col-md-4" v-for="(item,index) in mainData1.projects" :key="index">
                <div class="card p-3">
                    <p>{{item.title}}</p>
                    <p>{{item.des}}</p>
                    <a :href="item.link">Click Here</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import maindata from '@/assets/data/main.json'
    export default {
        name:'ProjectsHome',
        data:()=>({
            mainData1: maindata
        }),
        methods:{

        }
    }
</script>