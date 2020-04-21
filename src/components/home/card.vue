<template>
    <div class="card" style="width: 18rem;">
        <div class="card-body">
            <h5 class="card-title">{{data.title}}</h5>
            <h6 class="card-subtitle mb-2 text-muted">{{data.subtitle}}</h6>
            <p class="card-text">{{data.des}}</p>
            <a href="#" v-on:click="showData" class="card-link">Card link</a>
        </div>
    </div>
</template>

<script>
    export default {
        name:'CardComponennt',
        props:['data'],
        data:()=>({

        }),
        methods:{
            showData(){
                this.$emit('SuccessFunction')
            }
        }
    }
</script>