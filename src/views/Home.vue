<template>
  <div class="container">
    <div class="row">
      <div class="col-md-12">
        <p>Total ClICK = {{a}}</p>
        <HomeStartScreen/>
      </div>
    </div>
    <div class="row py-4">
      <div class="col-md-4">
        <CardComponent @SuccessFunction="showAlert" :data="cardData"/>
      </div>
      <div class="col-md-4">
        <CardComponent @SuccessFunction="showAlert" :data="cardData1"/>
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
import CardComponent from '@/components/home/card'
  export default {
    name:'HomeComponent23',
    components:{
      HomeComponent,
      HomeStartScreen,
      SkillsComponent,
      ProjectComponent,
      CardComponent
    },
    data:()=>({
      a:0,
      cardData:{
        title:'Tilte',
        subtitle:'Subtitle',
        des:'This is descriptionofthe cards'
      },
      cardData1:{
        title:'Tilte1',
        subtitle:'Subtitle1',
        des:'This is descriptionofthe cards1'
      },
    }),
    methods:{
      showAlert(){
        this.a =  this.a+1
        alert('Kuch to calling')
      }
    }
  }
</script>