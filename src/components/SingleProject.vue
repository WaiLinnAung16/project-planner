<template>
  <div class="project" @click="showDetail!=showDetail">
    <h3>{{project.title}}</h3>
    <p v-if="showDetail">{{project.detail}}</p>
  </div>
</template>

<script>
export default {
  name: "SingleProject.vue",
  props:["project"],
  data(){
    return{
      showDetail:false
    }
  },
}
</script>

<style scoped>
  .project{
    background-color: #f6f6f6;
    padding: 10px;
    margin: 10px 0;
    cursor:pointer;
  }
  .project h3{
    color: #0f6daa;
  }
</style>