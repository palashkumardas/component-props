<script setup>
import ToDo from "./components/ToDo.vue";
const slogan="Our Task List";
const mytasks = [
  { id: 1,title:"task one",done: true},
  {id: 2,title: "task two",done: true},
  {id: 3,title: "task three",done: true},
  {id: 4,title: "task four",done: false},
  {id: 5,title: "task five",done: false}

]
</script>
<template>
 <section class="mx-auto ">
    <h1 class="my-10 text-center">Components</h1>
    <div class="flex items-center justify-center h-[600px] font-medium">
      <div class="flex flex-grow items-center justify-center h-full text-gray-600 bg-gray-100">
        <!-- Component Start -->
        <ToDo :slogan="slogan" :tasks="mytasks"/>
        <!-- Component End  -->
      </div>
      
    </div>

  </section>
</template>

<style scoped>

</style>
