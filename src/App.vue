<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  <HomePage/>
  <CheckBox/>
  <CondtionalRandering/>
  <LoopingStatement/>
  <!-- <ChildComponent/> -->
   <ParentComponent/>
   <UserComponentB/>
   <HtmlBinding/>
   <ClassBinding/>
   <StudentComponent :name="name"/>
   <TeacherComponent name="Salam"/>
   <ChildToParentDataPassing :getUserDAta="getUserDAta"/>
   <RefKeyWord />
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import CheckBox from './components/CheckBox.vue';
import ChildToParentDataPassing from './components/ChildToParentDataPassing.vue';
import ClassBinding from './components/ClassBinding.vue';
// import ChildComponent from './components/ChildComponent.vue';
import CondtionalRandering from './components/CondtionalRandering.vue';
import HomePage from './components/HomePage.vue';
import HtmlBinding from './components/HtmlBinding.vue';
import LoopingStatement from './components/LoopingStatement.vue';
import ParentComponent from './components/ParentComponent.vue';
import RefKeyWord from './components/RefKeyWord.vue';
import StudentComponent from './components/StudentComponent.vue';
import TeacherComponent from './components/TeacherComponent.vue';
import UserComponentB from './components/UserComponentB.vue';



export default {
  name: 'App',
  components: {
    // HelloWorld,
    HomePage,
    CheckBox,
    CondtionalRandering,
    LoopingStatement,
    // ChildComponent,
    ParentComponent,
    UserComponentB,
    HtmlBinding,
    ClassBinding,
    StudentComponent,
    TeacherComponent,
    ChildToParentDataPassing,
    RefKeyWord,
    
  },
  data() {
    return {
      name:'Barkat'
    }
  },
  methods:
  {
    getUserDAta(data){
      this.name=data
    }
  }
}
</script>

