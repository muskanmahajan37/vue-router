<template>
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <HomeStartScreen/>
      </div>
    </div>

    <div class="row py-4" style="background-color:#e0e0e0">
      <div class="col-md-12">
        <SkillsComponent/>
      </div>
    </div>

    <div class="row py-4">
      <div class="col-md-12">
        <ProjectComponent/>
      </div>
    </div>

    <div class="row">
      <div class="col-md-12">
        <HomeComponent/>
      </div>
    </div>
    
    
  </div>
</template>

<script>
import HomeComponent from '@/components/home/header'
import HomeStartScreen from '@/components/home/homestartscreen'
import SkillsComponent from '@/components/home/skillset'
import ProjectComponent from '@/components/home/projects'
  export default {
    name:'HomeComponent23',
    components:{
      HomeComponent,
      HomeStartScreen,
      SkillsComponent,
      ProjectComponent
    },
    data:()=>({

    }),
    methods:{

    }
  }
</script>