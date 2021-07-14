

<script>
export default {
  name: 'Body',
  props: {
    show:{
        
        type:Boolean,
        default: false
        
    },
    

    course:{
        type:Object,
         default:() => {return{professor:'Pepito', name:'Mobile'}}
    },

    students:{
        type:Array,
        default:()=>{return ['Carlos','Pepito','Paula','Camila']}
    }
  }
}
</script>

<template>
  <div class="bod">
    <div class="row">
        <div class="col">
            <h1>V-if</h1>
            <div class="card w-75" v-if="show">
                <div class="card-body">
                    <h5 class="card-title">{{course.professor}}</h5>
                    <p class="card-text">{{course.name}}</p>
                </div>
            </div>
            <a v-on:click="show = !show" href="#" class="btn btn-primary">Button</a>
        </div>
        <div class="col">
            <h1>V-for</h1>
            <ul class="list-group">
                <li v-for="(student,i) in students" v-bind:key="student.ite">
                    {{i+1}}:{{student}}
                </li>
            </ul>
        </div>  
    </div>
  </div>
</template>




    
