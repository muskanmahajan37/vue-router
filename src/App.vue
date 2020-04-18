<template>
  <div>
    <Navbar/>
    <router-view></router-view>
  </div>
</template>

<script>
import Navbar from '@/components/common/navbar'
  export default {
    name:'MainComponent',
    components:{
      Navbar
    },
    data:()=>({

    }),
    methods:{

    }
  }
</script>